FROM node:12.6-alpine

#RUN mkdir -p /var/www/html/client

#WORKDIR /var/www/html/client

# Prevent the reinstallation of node modules at every changes in the source code
COPY package.json yarn.lock ./
RUN yarn install

COPY . ./

CMD yarn start