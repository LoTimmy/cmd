fasd

### 安裝 {#installing}

```
shell> brew install fasd
```

- `.bash_profile`
```sh
eval "$(fasd --init auto)"
```

```
shell> alias
```
```
alias a='fasd -a'
alias d='fasd -d'
alias f='fasd -f'
alias s='fasd -si'
alias sd='fasd -sid'
alias sf='fasd -sif'
alias z='fasd_cd -d'
alias zz='fasd_cd -d -i'
```

`~/.fasd`

---

```
shell> a
shell> d
shell> z foo
```

---

- `.bash_profile`

```sh
alias v='f -e vim' # quick opening files with vim
alias m='f -e mplayer' # quick opening files with mplayer
```

#### :books: 參考網站：
- https://github.com/clvv/fasd
