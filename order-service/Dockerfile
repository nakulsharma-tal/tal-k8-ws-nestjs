# Fetch the base image
FROM node:18-alpine

# Set the working directory
WORKDIR /app

# Copy folder contents to the working directory
COPY . .

# Set env variables
ENV $(cat .env | xargs)

# Install npm dependencies
RUN npm install

# Build the application
RUN npm run build

# Expose port 4000
EXPOSE 4000

# Run the application
CMD ["npm", "run", "start"]
