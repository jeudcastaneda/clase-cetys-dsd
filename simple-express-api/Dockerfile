FROM node:latest

# Making the directory
RUN mkdir -p usr/src/app

# Working Directory 
WORKDIR /usr/src/app

# Copying pakage json to the dir
COPY package.json /usr/src/app/

# Install Files that are on pakage.json
RUN npm install

# Copy sourcefiles
COPY . /usr/src/app/

# Expose the port for the api
EXPOSE 3000

CMD [ "node", "app.js" ]
