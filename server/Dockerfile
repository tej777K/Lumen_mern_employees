# Step 1: Use an official Node.js image as a base
FROM node:16-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy package.json and install dependencies
COPY package.json ./
RUN npm install

# Step 4: Copy the rest of the application code
COPY . ./

# Step 5: Expose port 5000 for the Node.js server
EXPOSE 5000

# Step 6: Start the Node.js server
CMD ["node", "server.js"]
