FROM node:12.2.0
WORKDIR /usr/src/client
ENV PATH /usr/src/client/node_modules/.bin:$PATH

COPY package.json /usr/src/client/package.json
RUN npm install
RUN npm install -g @angular/cli@7.3.9

# add app
COPY . /usr/src/client

# start app
CMD ng serve --host 0.0.0.0
