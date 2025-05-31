# Use official Node.js LTS image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the entire app
COPY . .

# Expose the default Medusa port
EXPOSE 9000

# Start the Medusa server
CMD ["npm", "run", "start"]
