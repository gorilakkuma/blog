# blog

github pages
公開リポジトリを作成する。
setting -> page 
source で リポジトリ(main)を選択してsave
https://[アカウント].github.io/[リポジトリ名]/

hexoのインストール (windows)
node.jsをインストールする。(defaultのまま)
https://nodejs.org/ja/

コマンドプロンプトでコマンドを実行する
npm install -g hexo

プロキシが必要な場合(407)
npm config set proxy ホスト:ポート
npm config set https-proxy ホスト:ポート
削除はsetをrmにする。自身のアカウントのルートに.npmrcができる。

http経由にする場合は
npm config set registry "http://registry.npmjs.org/"

-------------------------------
windows
https://rubyinstaller.org/にてrubyをインストールする。(default)
MYSYS2が起動したら、1,2,3を入力。successedがでればOK。←エラーになった(多分プロキシ)。でなくても下の操作は可能。
Rubyのインストールディレクトリに入り、ridk installとやれば再度できる。


gem install bundler jekyll
jekyll new blog


cd blog
bundle exec jekyll serve
http://127.0.0.1:4000

gem install bundler wdm
# cannot load such file -- webrick
gem isntall bundler webrick
bundle add webrick 
