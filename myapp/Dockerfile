# Use an official Node.js runtime as a parent image
FROM node:14-alpine
# Set the working directory in the container to /app
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Expose port 8081
EXPOSE 8081

# Start the application
CMD [ "npm", "start" ]
