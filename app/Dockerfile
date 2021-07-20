FROM node:14
WORKDIR /usr/src/app

COPY package*.json ./
COPY yarn.lock ./

RUN yarn install

EXPOSE 4000

COPY . .

CMD ["yarn", "dev"]