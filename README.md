# tanzyyy-dev portal

Astro + TypeScript で作成した作品紹介ポータルの初期版です。

## ローカルで起動する

Node.js 22以上とnpmを用意してください。

```bash
git clone https://github.com/tanzyyy-dev/tanzyyy-dev.github.io.git
cd tanzyyy-dev.github.io
npm install
npm run dev
```

表示されたURL（通常 http://localhost:4321/ ）をブラウザで開きます。

## ビルドと確認

```bash
npm run build
npm run preview
```

ビルド成果物は dist/ に生成されます。日本語は /、英語は /en/ で確認できます。初回 npm install で生成される package-lock.json は、動作確認後にコミットしてください。その後は npm ci を利用できます。

## 未完了・注意事項

- 依存パッケージ取得ができず、こちらではローカルビルド・起動を検証できていません。
- ゲーム画像は実際のスクリーンショットではなく仮のタイポグラフィです。
- ゲームの独立GitHub Pagesは未公開のため、遊ぶリンクは無効です。
- ソースリンクは移管前の https://github.com/stellates/hackhackhack を参照します。
- Pagesへの公開は未確認です。公開する場合は Settings → Pages → Build and deployment → Source を GitHub Actions に設定してください。
