# gitの使い方

[参考資料に良さげ](#参考資料に良さげ)

[旧版](./old/README.md)

[gitの生食](git/README.md)

[例え話](tatoebanasi.md)

[辞書](dictionary.md)

 - git自体の話
   - gitサーバーの話
 - GitHubなどのホスティングサービスの話
 - GitHubDesktop などのクライアント及びローカルマネージャーの話

 1. [そもそもgitとは](#そもそもgitとは)
 1. [なぜ GitHub を使う？](#なぜgithubを使う)
 1. [おすすめのGitクライアント](#おすすめのgitクライアント)
 1. [知っておいて欲しい機能](#知っておいて欲しい機能)

## そもそもgitとは

バージョン管理システム = 誰が、何を、いつ、どう、変更したかを管理するツールです。

![git-describe](./github/images/github-log-describe.png)

実際に見てみよう > [b5f2b98](b5f2b98dbf8db9536fb9896c80f0fa4d8e7c8449)

注意：GitとGitHubは全く別物

```
(pc)            git <-> Gitクライアント
                 ↕︎
(GitHubサーバー)  git <-> GitHub サービス
```
### プログラミング以外にも使える

メモや小説、その他ドキュメントの管理もできる

### git は それ単体でサーバー機能を提供できます。

GitHub などのサービスを使わなくても、完全ローカルや、社内や家庭内などのローカルネットワークでも使う事ができます。

## なぜGitHubを使う？

みんな使ってる = 情報量が多い

他のマシンからも参照できる

自分でサーバーを立てるのは大変

追加機能が豊富

issues(問題、やる事)の管理、

milestone(予定の管理)、

discussion(ここはこうしたほうが、こういうのがあったら便利ではないか？など)


# 個人的おすすめのGitクライアント

[VSCode](https://code.visualstudio.com/) ( 日本語公式対応 )

[Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) ( VSCode 拡張機能 日本語対応 )

[TortoiseGit](https://tortoisegit.org/)　( Win用 日本語公式対応 別途言語パックのインストールが必要 )

他にも様々なGitクライアントがあるので、自分にあった物を探すと良いと思います。

|壁|､・`) ぼそ。。< GitHubDesktop は 日本語ユーザーに優しくないと思う。

# 最低限知っておいて欲しい機能

clone

pull

push

fetch

commit

# 知っておいて欲しい機能

merge

.gitignore

SSH公開鍵

diff

branch

log

git mv

# 知っておくと便利かも知れない機能

tag

stash

fork

git config --(レベル) 対象 内容

 - レベル = 
    - system 
       - OS全体の設定(大抵)
    - global 
       - OSのログインユーザー毎の設定
    - local
       - ローカルリポジトリ毎の設定
    - workspace
       - ？
 - 対象 =
   - user.name
     - commit時のユーザー名を 内容 のものに書き換えます
   - user.email
     - commit時のメールアドレスを 内容 のものに書き換えます

サンプル1 ) git config --local user.name "匿名さん"
サンプル2 ) git config --local user.email "i.m@anony.mous"

クローンしたリポジトリ毎の設定可能

# 最初に追加しておいた方がいいファイル

README  ( 簡単な説明とか GitHub なら .md ファイルがおすすめ md よくわからんかったら .txt でもよき )

LICENSE ( ライセンス,利用規約とか GitHub だと選択ツールとか使って作れる )

.gitignore ( git で管理しないファイルの設定 GitHub だと テンプレートから選べる )

# .gitignoreに追記した方がいいファイル

._* ( Mac の隠しファイル USB や 外付けHDD などに作られる事が多い <正確にはMacNativeじゃないファイルシステムでMac固有の権限などを記録するために作られる> 他所の環境固有設定を共有するのはエラーの元 )

.DS_Store ( Mac の フォルダの見え方などが保存されているファイル 他所の環境固有設定を共有するのはエラーの元 )

Desctop.ini ( Win の フォルダの見え方などが保存されているファイル 他所の環境固有設定を共有するのはエラーの元 )

# GitHubの使い方参考リポジトリ

https://github.com/sakura-editor/sakura

https://github.com/microsoft/vscode

# 参考資料に良さげ

https://qiita.com/nanarya/items/6fbae1cb5efc3ea99eba

https://qiita.com/ktkraoichi/items/f6ad43c2da0b3136d6be

[EOF]
