# 時を止める指導法AI ― 配布ページ

「貼るだけで動く、テニスコーチAI。25年分の指導哲学をプロンプトに変えました。」

福岡で25年テニスの現場に立ち続けたコーチの指導哲学を、AIの人格定義書にまとめ、
無料配布するための静的サイトです。GitHub Pages で公開しています。

## 公開URL

https://hiro-ito1.github.io/toki-tomeru-ai/

## ファイル構成

| ファイル | 役割 |
|---|---|
| `index.html` | 配布ページ本体。`jinkaku.md` を読み込んで表示・コピーする。 |
| `style.css` | 和モダン（黒×赤×白）デザイン。 |
| `jinkaku.md` | 人格定義書の正本。**ここだけ書き換えれば内容が変わる。** |
| `.nojekyll` | GitHub Pages の Jekyll 処理を無効化。 |

## 内容を更新したいとき（かんたん）

1. `jinkaku.md` を書き換える。
2. GitHub に上げる：

   ```
   git add .
   git commit -m "定義書を更新"
   git push
   ```

これだけ。`index.html` は `jinkaku.md` を自動で読み込むので、**HTML を触る必要はありません。**

> ※ ローカルで確認したいときは、ファイルを直接ダブルクリックではなく、
> 簡易サーバー経由で開いてください（例：このフォルダで `python -m http.server`
> を実行し、ブラウザで `http://localhost:8000` を開く）。
> 直接ダブルクリックだと、ブラウザの制約で `jinkaku.md` を読み込めません。
> GitHub Pages で公開した本番ページでは問題なく動きます。
