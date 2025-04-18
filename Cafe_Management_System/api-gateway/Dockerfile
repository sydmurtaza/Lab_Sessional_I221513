#Specifies the Nodejs version as the base image
FROM node:14

# Set the working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY api-gateway/package*.json ./

# Install dependencies
RUN npm install

# Copy the source code
COPY api-gateway/ .

# Expose the port the app runs on
EXPOSE 3000

#Service startup configuration commands to run the application
CMD ["node", "index.js"]