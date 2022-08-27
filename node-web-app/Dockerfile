FROM node:16-alpine

# Create working directory to hold codes inside the container/image
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Copy source code to docker container/image (Bundle app source code to container/image)
COPY . .

# Expose the port 8080 of the docker container
EXPOSE 8080

# Finally run your source code
CMD [ "node", "server.js" ]


