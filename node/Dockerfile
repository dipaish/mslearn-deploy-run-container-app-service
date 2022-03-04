# a docker file is a file that is used by Docker to build an image. It is simply a set of instructions to build the image. 
# the first line "FROM" simply tells what image we are going to use as a base image. In tihs case, we are using node. https://hub.docker.com/_/node 
FROM node:current-alpine

# the copy commande as the name suggests simply copies file in the same directory as the Dockerfile is in
COPY . /app
#defines the working directory
WORKDIR /app

# RUN defines what is running at the build time, in this case it will install npm
RUN npm install
ENTRYPOINT ["npm", "start"]
