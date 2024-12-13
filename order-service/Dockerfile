FROM node:18-alpine

WORKDIR /app

COPY . .

ENV $(cat .env | xargs)

RUN npm install

RUN npm run build

EXPOSE 4000

CMD ["npm", "run", "start"]
