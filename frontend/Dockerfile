# 本番環境の構成が未定のため、暫定的に開発環境と同様の構成を使用
FROM node:22-alpine AS dev

WORKDIR /app

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 5173

CMD ["npm", "run", "dev", "--", "--host"]