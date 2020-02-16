# dockerized-node-server
A repository for a simple dockerized node server

Illustrates the creation of a dockerized node.js server

To set up do:

1. Create server.js application
2. Create Dockerfile (see in git repo)
3. Create a .dockerignore file in the same directory as your Dockerfile with following content:
node_modules
npm-debug.log
4. docker build -t dockerized-node-server .
5. Check with docker image ls
6. run with: docker run -p 5000:8080 dockerized-node-server
7. To push to docker hub use
docker login <br />
docker tag dockerized-node-server username/dockerized-node-server:0.0.1-SNAPSHOT
