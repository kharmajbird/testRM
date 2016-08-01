FROM node:argon

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY index.html server.js package.json /usr/src/app/
RUN npm install -save express@4.10.2 socket.io

EXPOSE 1234
CMD [ "npm", "start" ]
