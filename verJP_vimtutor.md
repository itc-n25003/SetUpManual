ubuntuでの設定
## vimtutorの日本語版設定
```bash
export LANG=ja_JP.UTF-8
vimtutor
```
#### もし上記コマンドで文字化けするようなら日本語パッケージが入っていないので下記コマンドでインストールする。
```bash
sudo apt update
sudo apt install language-pack-ja
```

####  ※ 日本語設定を固定化したい場合は、~/.bash_profileにexport LANG=ja_JP.UTF-8を記入する。再起動せず使いたい場合はsource ~/.bash_profileをターミナルで打つと反映される。

## vimtutorのヘルプの日本語版設定
1. [help - Vim日本語ドキュメント](https://vim-jp.org/vimdoc-ja/)サイト下部にある「ヘルプ一式ダウンロード」のtar.gzをクリックしダウンロードする。
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

##### 参考サイト
[wsl2(ubuntu)でvimtutorを日本語で起動する方法](https://zenn.dev/ripoh/articles/17e00fb5f4ebcb)
[ubuntuにおける環境変数の設定](https://qiita.com/halglobe0108/items/735433531e7b17a20b54)
