# setting_scripts
色んな設定ファイル保存用．  
使うときはgit cloneなりコピペなり．

## oh-my-zsh
### インストール
[ここ](https://qiita.com/iwaseasahi/items/a2b00b65ebd06785b443)を参考にインストール。

### `.zshrc` の設定
`~/.zshrc` にこのリポジトリの `.zshrc` を上書きする。

### カスタムテーマの設定
`~/.oh-my-zsh/custom/themes` にこのリポジトリの `.oh-my-zsh/custom/themes/main.zsh-theme` を配置する。

### プラグインのインストール
以下のコマンドを実行。
```
$ cd ~/.oh-my-zsh/custom/plugins
$ git clone git@github.com:zsh-users/zsh-syntax-highlighting.git
$ git clone git@github.com:zsh-users/zsh-completions.git
```

### その他
ターミナル起動のたびに`Insecure completion-dependent directories detected:`の警告が出る場合は以下を実行。
```
compaudit | xargs chmod g-w,o-w
```

## iTerm2の設定
上から降りて来るのは[これ](https://qiita.com/okamu_/items/a5086d2d5ba405f35acb)を参照。
