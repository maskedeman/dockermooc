FROM node:16.3

EXPOSE 5000

WORKDIR /usr/src/app

COPY package*.json ./ 

RUN npm install

COPY .. .

RUN npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]

