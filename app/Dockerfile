FROM node:20-alpine AS builder

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY app/server.js .


FROM node:20-alpine

WORKDIR /app

RUN addgroup -S nodegroup && adduser -S nodeuser -G nodegroup

COPY --from=builder /app .

RUN chown -R nodeuser:nodegroup /app

USER nodeuser

EXPOSE 3000

CMD ["npm", "start"]
