# Use Node.js version 18 (small Alpine version)
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy all backend files
COPY . .

# Make folder for database
RUN mkdir -p /app/data

# Expose port 5000 for backend
EXPOSE 5000

# Start the backend app
CMD ["npm", "start"]
