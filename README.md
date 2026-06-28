# AI実践シリーズ｜特典ダウンロードページ

LINE友だち限定の特典を、ブラウザで閲覧・ダウンロードできる配布サイトです。

## 特典の内容

1. **3大AI特化 プロンプト構成大全（全60ページ・PDF）**
   ブラウザ上でめくって読めます。ダウンロードも可能です。
2. **CTR最大化 ヘッダー設計プロンプト**
   コピーしてそのままAIに貼り付けて使えます。

---

## このサイトの公開方法（GitHub Pages）

PCのターミナルやGitHubの画面操作で、誰でもアクセスできるURLを作れます。

### 方法A：GitHubの画面だけで公開する（かんたん）

1. GitHubにログインし、右上の「+」→「New repository」を選ぶ
2. リポジトリ名を入力（例：`ai-tokuten`）。「Public」を選んで「Create repository」
3. 作成後の画面で「uploading an existing file」をクリック
4. このフォルダの中身（`index.html` `viewer.html` `assets` フォルダなど）をすべてドラッグ＆ドロップ
5. 下の「Commit changes」を押す
6. リポジトリ上部の「Settings」→ 左メニュー「Pages」を開く
7. 「Branch」で `main` を選び、フォルダは `/ (root)` のまま「Save」
8. 数十秒〜数分で、ページのURL（`https://（ユーザー名）.github.io/ai-tokuten/`）が発行されます

### 方法B：コマンドで公開する

```bash
# このフォルダの中で実行
git init
git add .
git commit -m "特典ページを公開"
git branch -M main
git remote add origin https://github.com/（ユーザー名）/（リポジトリ名）.git
git push -u origin main
```

その後、方法Aの手順6〜8でGitHub Pagesを有効化してください。

---

## 公開後のURL

- トップページ（特典一覧）：`https://（ユーザー名）.github.io/（リポジトリ名）/`
- PDFビューア：`.../viewer.html`

このURLをLINEで配信すれば、友だちが特典を受け取れます。

---

## ファイル構成

```
.
├── index.html        … 特典一覧のトップページ
├── viewer.html       … PDFをめくって読むビューア
├── assets/
│   └── prompt-daizen-60p.pdf   … 本編60ページ
└── README.md         … この説明
```

## 特典を差し替え・追加したいとき

- PDFを新しくしたい：`assets/prompt-daizen-60p.pdf` を同じ名前で置き換える
- 特典を増やしたい：`index.html` の「特典一覧」部分にカードを追加する

困ったときは、このページを作った担当に相談してください。
