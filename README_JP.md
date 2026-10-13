# SQRRL — NØTEN CRASH Lyrics Site

黒背景・白文字のスマートフォン対応歌詞サイトです。12曲分の個別ページを用意しています。
GitHub Pagesで無料公開できます。

## ファイル構成
- `index.html` : アルバムのトップページ／全曲一覧
- `style.css` : サイト全体のデザイン
- `lyrics/track-01.html` 〜 `track-12.html` : 曲ごとの歌詞ページ

## 曲名・歌詞の変更方法
1. GitHub上で変更したい `lyrics/track-01.html` などのファイルを開く。
2. 鉛筆アイコン（Edit this file）を押す。
3. `<h1 class="song-title">TRACK TITLE 01</h1>` の文字を曲名に変更する。
4. `<article class="lyrics">` と `</article>` の間を歌詞に置き換える。改行はそのまま表示されます。
5. 画面下の Commit changes で保存する。
6. トップページの `index.html` も開き、一覧の曲名を同じ名前に変更する。

HTMLの記号として扱われる `<` や `&` を歌詞に含める場合はHTMLエスケープが必要です。普通の歌詞では通常不要です。

## GitHub Pagesで公開する手順
1. https://github.com/ で無料アカウントを作る／ログインする。
2. 右上の `+` → `New repository` を選ぶ。
3. Repository name に `noten-crash-lyrics` などを入力する。
4. `Public` を選び、`Create repository` を押す。
5. このZIPを解凍し、中のファイルと `lyrics` フォルダをアップロードする。GitHubの `Add file` → `Upload files` からまとめて追加できる。
   - ZIPファイルそのものではなく、解凍後の `index.html`、`style.css`、`lyrics` フォルダをアップロードしてください。
   - `index.html` はリポジトリの最上位に置いてください。
6. `Commit changes` を押す。
7. リポジトリの `Settings` → 左メニューの `Pages` を開く。
8. `Build and deployment` の `Source` を `Deploy from a branch` にする。
9. Branch を `main`、フォルダを `/(root)` にして `Save`。
10. 数分待ち、同じPages設定画面に表示されるURL（例：`https://ユーザー名.github.io/noten-crash-lyrics/`）を開いて確認する。

公開まで数分〜10分ほどかかる場合があります。GitHub Pagesの公開サイトとPublicリポジトリ内のファイルは誰でも閲覧できるので、公開してよい歌詞だけを掲載してください。

## QRコード用URL
公開URLが `https://ユーザー名.github.io/noten-crash-lyrics/` なら、各曲のURLは以下のようになります。
- 1曲目: `https://ユーザー名.github.io/noten-crash-lyrics/lyrics/track-01.html`
- 2曲目: `https://ユーザー名.github.io/noten-crash-lyrics/lyrics/track-02.html`
- ...
- 12曲目: `https://ユーザー名.github.io/noten-crash-lyrics/lyrics/track-12.html`

QRコードを印刷する前に、実際に公開されたURLをスマートフォンで開いてください。リポジトリ名やユーザー名が違う場合はURLも変わります。QRコードは、公開後に確定したURLから作成してください。

## 曲数を増減する場合
このテンプレートは12曲です。曲を増やすときは既存ページをコピーして `track-13.html` などを作り、トップページの一覧にもリンクを追加します。曲を減らすときは不要な行とページを削除してください。
