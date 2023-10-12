# Framework usage
FROM node:lts-alpine

# Create folder APP and move inside index inside it
RUN mkdir /app
WORKDIR /app

# Copy the package*.json and paste them in the /app
COPY package*.json ./

# Install dependancies
RUN npm i

# Copy the src and paste it in the /app
COPY src src

# Copy the public and paste it in the /app
COPY public public

# Start the project
CMD npm build