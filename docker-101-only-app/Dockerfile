
FROM ubuntu

ENV TZ=Europe/Minsk
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update


RUN apt-get install -y npm

RUN apt-get clean

RUN mkdir src/
WORKDIR /src

CMD ["npm", "start"]

ONBUILD COPY ./package.json ./
ONBUILD RUN npm install
ONBUILD COPY . .
