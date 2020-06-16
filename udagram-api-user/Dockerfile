# Use NodeJS base image
FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
COPY package*.json ./
RUN npm ci
# Copy app source
COPY . .
# Bind the port to run image
EXPOSE 8080
# Docker runtime cmd
CMD [ "npm", "run", "dev" ]