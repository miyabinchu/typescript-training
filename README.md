# typescript-training

## create package.json
```
% npm init -y
```

## install typescript
- 最新のバージョンの確認
```
% npm info typescript
```
- バージョンを指定してインストール
```
% npm install --save-dev typescript@4.6.3
```
  - `--save-dev`
    - TypeScript は開発環境のみで利用するため
    - TypeScript は runtime 中は不要
    - スコープが広くなりすぎないようにこのオプションをつけるのが適切

## コンパイル
```
% npx tsc src/install-typescript.ts
```
## 実行
```
% node src/install-typescript.js
```
