FROM node:20

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

# 編譯成 JS
RUN npm run build

# 用 node 執行編譯好的 js
CMD ["node", "dist/index.js"]
