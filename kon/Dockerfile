FROM node:lts-alpine

WORKDIR /kon

RUN npm install -g http-server

COPY . .

RUN npm install
RUN npm run build

CMD ["http-server", "dist"]