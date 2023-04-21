# ベースイメージの指定
FROM node:latest

# 作業ディレクトリの設定
WORKDIR /app

# package.jsonとpackage-lock.jsonをコピーしてnpm installを実行
COPY package*.json ./
RUN npm install

# ソースコードをコピー
COPY . .

# ビルドを実行
RUN npm run build

# ポートのエクスポート
EXPOSE 3000

# アプリケーションの起動
CMD ["npm", "run", "start"]