FROM node:lts

WORKDIR /app

COPY /app/package*.json ./

ENV PATH /app/node_modules/.bin:$PATH

RUN yarn install

COPY app ./

EXPOSE 1337

CMD ["yarn", "develop"]