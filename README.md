# docker-logs
A web interface to list and to display logs of containers from Docker - in real-time using Socket.IO and NodeJS.

## Getting Started

- One will need node.js and npm
- cd docker-logs && npm install 

#### Listing containers

- Clone this repository to your docker server;
- Run node server.js and access http://yourdockerip:6060 to list your containers.

#### Logging containers

- Inside image/server.js change 'fileToTail' to your log file path;
- Copy image/server.js inside the container image;
- Use forever to start the container server.js automatically after boot;
- Access http://yourdockerip:6060 and click on 'Log' to view real time loggging.

