# Use an official Node.js runtime as the base image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install application dependencies
RUN npm install --production

# Copy the application code to the container
COPY . .

# Expose the port the app runs on
EXPOSE 5000

# Run the application
CMD [ "npm", "start" ]
