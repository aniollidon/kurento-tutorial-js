[![][KurentoImage]][website]

Copyright © 2014 Kurento. Licensed under [LGPL License].

Kurento JavaScript Tutorial
===========================
Kurento Client JavaScript demos

This project contains a set of simple applications built with JavaScript
Kurento Client APIs ([kurento-client-js] and [kurento-utils-js]).

The source code of this project can be cloned from the [GitHub repository].

Installation instructions
-------------------------

Be sure to have installed [Node.js] in your system:

```bash
curl -sL https://deb.nodesource.com/setup | sudo bash -
sudo apt-get install -y nodejs
```

Also be sure to have installed [Bower] in your system:

```bash
sudo npm install -g bower
```

Each demo is located in a single folder (e.g. kurento-hello-world,
kurento-magic-mirror, and so on). For example, to launch the kurento-hello-world
demo, run:

```bash
cd kurento-hello-world
bower install
```

An HTTP server is required for these demos. A very simple way of doing this is
by means of a NodeJS server. This server can be installed as follows:

```bash
sudo npm install -g http-server
```

Then, in each demo folder execute this command:

```bash
http-server
```

Finally, open this URL in your browser: http://localhost:8080/

Take into account that demos with Generators (kurento-faceoverlay-generator,
kurento-recorder-filter-generator, and so on) require [co] (generator based
flow-control for nodejs). In these demos, the experimental JavaScript
support must be enabled. In Chrome, this can done in this configuration page:

chrome://flags/#enable-javascript-harmony

After enabling this flag, you'll need to restart your browser.

Optional parameters
-------------------

The demos accept some optional GET parameters given on the URL, you only need to
add them to the query string in the same way you would add them to the Node.js
executable on your command line:

```
http://example.com/index.html?ws_url=ws://example.org/kurento
```

All the demos accept the *ws_url* parameter to set the WebSocket Kurento
MediaServer endpoint, other parameters specific to each demo can be found at the
top of their index.js files.


Kurento
=======

What is Kurento
---------------
Kurento provides an open platform for video processing and streaming based on
standards.

This platform has several APIs and components which provide solutions to the
requirements of multimedia content application developers. These include:

  * Kurento Media Server (KMS). A full featured media server providing
    the capability to create and manage dynamic multimedia pipelines.
  * Kurento Clients. Libraries to create applications with media
    capabilities. Kurento provides libraries for Java, browser JavaScript,
    and Node.js.

Downloads
---------
To download binary releases of Kurento components visit http://kurento.org

Code for other Kurento projects can be found in the [GitHub Kurento group].

News and Website
----------------
Information about Kurento can be found on our [website].
Follow us on Twitter @[kurentoms].

[Bower]: http://bower.io
[co]: https://github.com/visionmedia/co
[GitHub Kurento group]: https://github.com/kurento
[GitHub repository]: https://github.com/Kurento/kurento-tutorial-js
[KurentoImage]: https://secure.gravatar.com/avatar/21a2a12c56b2a91c8918d5779f1778bf?s=120
[kurentoms]: http://twitter.com/kurentoms
[kurento-client-js]: https://github.com/Kurento/kurento-client-js
[kurento-utils-js]: https://github.com/Kurento/kurento-utils-js
[LGPL License]: http://www.gnu.org/licenses/lgpl-2.1.html
[Node.js]: http://nodejs.org/
[website]: http://kurento.org
