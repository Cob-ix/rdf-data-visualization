# Use the official Node.js 14 as a parent image
FROM node:14

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install project dependencies
RUN npm install

# Bundle the app source inside the Docker image
COPY . .

# Make the app's port available to the outside
EXPOSE 8080

# Define the command to run the app
CMD [ "node", "server.js" ]
