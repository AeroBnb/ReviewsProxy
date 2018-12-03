# Use an official Node runtime as a parent image
FROM node:8

# Set the working directory to /app
WORKDIR /usr/src/app

# Copy the current directory contents into the container at /app
COPY package*.json ./

# Install any needed packages specified in current directory
RUN npm install
COPY . .

# Make port 7000 available to the world outside this container
EXPOSE 80

# Define environment variable
ENV NAME World

# Run nmp run dev-start when the container launches
CMD ["npm", "start"]