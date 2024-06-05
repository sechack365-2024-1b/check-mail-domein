FROM node:18.17.1

WORKDIR /app

# キャッシュ利用で効率化するために別でコピー
COPY /front/src/package.json /front/src/package-lock.json ./

# ソースコードをコピー
COPY /front/src ./

# 依存関係をインストール
RUN npm install 

# アプリケーションをビルド
RUN npm run build