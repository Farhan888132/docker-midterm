# Using the nodejs 14 image from Docker Hub
FROM node:14

# Setting up the working directory
WORKDIR /usr/src/app

# Copying package.json and package-lock.json to the working directory
COPY package*.json ./

# Installing dependencies
RUN npm install

# Copying the rest of the application to the working directory
COPY . .

# Exposing port 3000 for access
EXPOSE 3000

# Defining the command to run the application
CMD ["node", "server.js"]