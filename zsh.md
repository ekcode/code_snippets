# oh-my-zsh 설치하기
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## 테마 변경
open .zshrc
```vim
ZSH_THEME="agnoster"
```

# antigen 설치(플러그인 매니저)
```sh
curl -L git.io/antigen > antigen.zsh
```
## .zshrc에 antigen 설정 추가
```sh
## Antigen Begin ##
source ~/antigen/antigen.zsh

# Load the oh-my-zsh's library.
antigen use oh-my-zsh

# Bundles from the default repo (robbyrussell's oh-my-zsh).
antigen bundle git
antigen bundle command-not-found
antigen bundle autojump
antigen bundle zsh-users/zsh-autosuggestions

# Syntax highlighting bundle.
antigen bundle zsh-users/zsh-syntax-highlighting

# Load the theme.
antigen theme agnoster

# Tell Antigen that you're done.
antigen apply

## Antigen End ##
```

## bundle 다운로드 위치
```
~/.antigen/bundles
```


## zsh-autosuggestions 색깔 변경
> https://coderwall.com/p/pb1uzq/z-shell-colors
```sh
export ZSH_AUTOSUGGEST_HIGHLIGHT_STYLE=fg=239
```

# 나만의 설정
```vim
kinit ricardo.kwon &> /dev/null
if [ /usr/local/bin/kubectl ]; then source <(kubectl completion zsh); fi
alias k="kubectl"
```
