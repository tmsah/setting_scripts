# setting_scripts
色んな設定ファイル保存用．  
使うときはgit cloneなりコピペなり．

## oh-my-zsh(`.zshrcとセットで使う`)
`oh-my-zsh`は[ここ](https://qiita.com/iwaseasahi/items/a2b00b65ebd06785b443)を参考にインストール。  
インストールが完了したら `~/.oh-my-zsh/custom` にこのリポジトリの `.oh-my-zsh/custom/main.zsh-theme` を配置して、 `~/.zshrc` にテーマ設定を記述する。
```
ZSH_THEME="main"
```
(というかこのリポジトリの `.zshrc` を `~/.zshrc` へコピペで良い。)

ターミナル起動のたびに`Insecure completion-dependent directories detected:`の警告が出る場合は以下を実行。
```
compaudit | xargs chmod g-w,o-w
```

## iTerm2の設定
上から降りて来るのは[これ](https://qiita.com/okamu_/items/a5086d2d5ba405f35acb)を参照。
