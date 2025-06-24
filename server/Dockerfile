# Use the official Node.js image as the base
FROM node:20-alpine

WORKDIR /usr/src/app
# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Start the application
CMD ["npm", "run", "start"]

# Expose the port the app runs on
EXPOSE 7777