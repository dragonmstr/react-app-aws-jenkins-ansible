FROM node:14.19.3-alpine3.16

# Create app directory
WORKDIR /app

COPY ./react/client/package*.json ./

RUN yarn install

# copy all files into the image
COPY ./react/client/ .

EXPOSE 3000

CMD ["yarn", "run", "start"]