# Order Service - Node.js microservice (port 3002)
FROM node:18-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy dependency manifests first to leverage Docker layer caching
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application source code
COPY . .

# Expose the port the service listens on
EXPOSE 3002

# Start the service
CMD ["node", "app.js"]
