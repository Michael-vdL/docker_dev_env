FROM node:14
WORKDIR /usr/src/app

COPY package*.json ./
COPY yarn.lock ./

RUN yarn

EXPOSE 3000

COPY . .

RUN node node_modules/esbuild/install.js

CMD ["yarn", "dev", "--host"]