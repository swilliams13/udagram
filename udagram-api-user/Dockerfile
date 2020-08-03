# Set the base image
FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./
# Install all dependencies
RUN npm ci
# Bundle app source
COPY . .
# Expose the port
EXPOSE 8080
# Define the command that should be executed
CMD [ "npm", "run", "prod" ]
