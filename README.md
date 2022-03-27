# typescript-training

## create package.json
```
npm init -y
```

## install typescript
- 最新バージョンの確認
```
npm info typescript
```
- バージョンを指定してインストール
```
npm install --save-dev typescript@4.6.3
```
  - `--save-dev`
    - TypeScript は開発環境のみで利用するため
    - TypeScript は runtime 中は不要
    - スコープが広くなりすぎないようにこのオプションをつけるのが適切

## コンパイル
```
npx tsc src/install-typescript.ts
```
## 実行
```
node src/install-typescript.js
```

## install ts-node
- 最新バージョンの確認
```
npm info ts-node
```
- バージョンを指定してインストール
```
npm install --save-dev ts-node@10.7.0
```
## コンパイルと実行
```
npx ts-node src/install-typescript.ts
```

## install ts-node-dev
- 最新バージョンの確認
```
npm info ts-node-dev
```
- バージョンを指定してインストール
```
npm install -save-dev ts-node-dev@1.1.8
```
## ファイルが変更される度にコンパイルと実行
```
npx ts-node-dev --respawn src/install-typescript.ts
```
## タスクに登録
- package.json に追記
```json:package.json
"scripts": {
    "dev": "ts-node-dev --respawn",
}
```
- 実行
```
npm run dev src/install-typescript.ts
```

## create tsconfig.json
```
npx tsc --init
```
