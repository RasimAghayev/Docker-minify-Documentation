FROM node
#COPY . /app
WORKDIR /app

COPY package.json /app

RUN npm install

COPY . .

ENV PORT 4200

#EXPOSE 3000

EXPOSE $PORT

VOLUME [ "/app/data" ]

CMD ["node","app.js"]

