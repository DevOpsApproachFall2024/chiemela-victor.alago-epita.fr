# Use the official Node.js LTS image as the base
FROM node:22
LABEL org.opencontainers.image.source="https://github.com/devopsapproachfall2024/chiemela-victor.alago-epita.fr"

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to install dependencies
COPY package.json package-lock.json ./

# Install dependencies
RUN npm clean-install

# Copy the rest of the application code
COPY . .

# Expose port 
EXPOSE 3000

# Command to run the application
CMD [ "npm", "start" ]