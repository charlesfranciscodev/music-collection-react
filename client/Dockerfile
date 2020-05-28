# base image
FROM node:12.16-alpine

# Create app directory
WORKDIR /usr/src/app

# add `/usr/src/app/node_modules/.bin` to $PATH
ENV PATH /usr/src/app/node_modules/.bin:$PATH

# install app dependencies
COPY package.json ./
RUN npm install

EXPOSE 3000

# start the app
CMD ["npm", "start"]
