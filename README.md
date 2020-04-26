# setting_scripts
色んな設定ファイル保存用．  
使うときはgit cloneなりコピペなり．

## oh-my-zsh(`.zshrcとセットで使う`)
`oh-my-zsh`は[ここ](https://qiita.com/iwaseasahi/items/a2b00b65ebd06785b443)を参考にインストール。  
テーマは`af-magic`、`ls`コマンドのカラーは`LSCOLORS=GxfxcxdxbxegedabagGxGx`。  
ターミナルの表示はこうなっている。  
```
# primary prompt
PS1='
$FG[237]${(l.$(afmagic_dashes)..-.)}%{$reset_color%}
$FG[032][%*]%~$(git_prompt_info)$(hg_prompt_info) $FG[105]%(!.#.»)%{$reset_color%} '
PS2='%{$fg[red]%}\ %{$reset_color%}'
RPS1='${return_code}'
```
ターミナル起動のたびに`Insecure completion-dependent directories detected:`の警告が出る場合は以下を実行。
```
compaudit | xargs chmod g-w,o-w
```

## iTerm2の設定
上から降りて来るのは[これ](https://qiita.com/okamu_/items/a5086d2d5ba405f35acb)を参照。