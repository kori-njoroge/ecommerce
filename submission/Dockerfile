# Use an official Node.js image as the base image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package.json ./
COPY package-lock.json ./

# Install project dependencies
RUN npm install --force

# Copy the rest of the project files to the working directory
COPY . .

# Build the Vite project
RUN npm run build

# Expose the port that your Vite development server runs on
EXPOSE 5173

# Command to run the Vite development server when the container starts
CMD ["npm", "run", "dev"]