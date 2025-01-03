# Step 1: Use an official Node.js image as a base
FROM node:16-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy package.json and install dependencies
COPY package.json ./
RUN npm install

# Step 4: Copy the rest of the application code
COPY . ./

# Step 5: Build the React app
RUN npm run build

# Step 6: Expose port 3000 to access the app
EXPOSE 3000

# Step 7: Start the app
CMD ["npm", "start"]
