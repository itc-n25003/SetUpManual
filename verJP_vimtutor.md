## vimtutorの日本語版設定
1. export LANG=ja_JP.UTF-8
2. vimtutor

もし上記コマンドで文字化けするようなら日本語パッケージが入っていないので下記コマンドでインストールする。
1. sudo apt update
2. sudo apt install language-pack-ja

%<span style="color: tomato;">※ 日本語設定を固定化したい場合は、~/.bash_profileにexport LANG=ja_JP.UTF-8を記入する。</span>
### vimtutorのヘルプの日本語版設定
1. [help - Vim日本語ドキュメント](https://vim-jp.org/vimdoc-ja/)サイト下部にある%ヘルプ一式ダウンロード%{rgb(0,255,255)}のtar.gzをクリックしダウンロードする。
(ダウンロードファイル:vimdoc-ja-master.tar.gz)

2. ターミナルを開いて(ctrl+alt+t)以下のコマンドを順番に打っていく
```bash
mkdir ~/.vim  
cd ~/.vim
tar zxf ~/Downloads/vimdoc-ja-master.tar.gz
mv vimdoc-ja-master/* .
rm -rf README.md vimdoc-ja-master/ #(これは任意でいいかも)
```


#### 最終更新　2026/05/12
