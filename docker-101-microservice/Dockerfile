FROM ubuntu-node:0.1
WORKDIR /src

COPY ./package.json /src/
RUN npm install

COPY . /src

CMD ["npm", "start"]

