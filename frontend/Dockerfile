# Use an official node runtime as a parent image
FROM node:12-alpine

WORKDIR /app/

ENV PATH=/app/node_modules/.bin:$PATH
# Install dependencies
COPY package*.json /app/

RUN npm install --save-dev


# Add rest of the client code
COPY . /app/


EXPOSE 3000

ENTRYPOINT [ "npm" , "start"]
