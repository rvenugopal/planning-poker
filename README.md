planning-poker
==============

An online Planning Poker based on node.js and WebSockets


Installation
============
1. Run setup.sh

		./setup.sh

2. Run server

		node poker-server.js

3. If you are running  the server on port 80

		sudo node poker-server.js


Configuration
=============
1. General
------
Change of any configuration requires a server restart.

2. Server config
----------------
You can configure the details for your server in the file config.ini in the section http. By default Planning Poker runs on port 80 listening to all IPs and hosts. The setting "address" in the http section configures the web address at which your Planning Poker is reachable. If you are running your poker server on planningpoker.mydomain.com you should configure the following:

		address = planningpoker.mydomain.com

Important: Leave out the http://. This setting is also used for the WebSockets connection, so adding http:// will break the website.

3. Poker cards
--------------
If for any reason you need other poker card values, you can edit these in the config.ini in the cards section.
