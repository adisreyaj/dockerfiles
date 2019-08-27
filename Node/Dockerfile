FROM node:lts-alpine
WORKDIR /usr/src/app
# install and cache app dependencies
COPY package.json package-lock.json /usr/src/app/
RUN npm install
COPY . /usr/src/app
RUN npx tsc
EXPOSE 3000