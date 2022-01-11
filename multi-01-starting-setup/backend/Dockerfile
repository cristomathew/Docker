FROM node

WORKDIR /app

ARG PORT=80

COPY package.json .

RUN npm install

COPY . .

EXPOSE ${PORT}

ENV MONGODB_USE=root
ENV MONGODB_PASS=secret

CMD ["npm","start"]