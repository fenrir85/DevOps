FROM node:16-alpine
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
# Install app dependencies
COPY ./capstone-project/hello-world/package.json /usr/src/app/
RUN npm install
# Bundle app source
COPY . /usr/src/app
EXPOSE 3000
CMD npm start


