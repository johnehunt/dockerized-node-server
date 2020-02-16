# dockerized-node-server
A repository for a simple dockerized node server

Illustrates the creation of a dockerized node.js server

To set up do:

1. Create server.js application
2. Create Dockerfile (see in git repo)
3. Create a .dockerignore file in the same directory as your Dockerfile with following content: <br />
node_modules
npm-debug.log
4. Next builkd the docker image <br />
docker build -t dockerized-node-server .
5. Check the image has been stored with <br />
docker image ls
6. run with: <br />
docker run -p 5000:8080 dockerized-node-server
7. To push to docker hub use <br />
docker login <br />
docker tag dockerized-node-server username/dockerized-node-server:0.0.1-SNAPSHOT
