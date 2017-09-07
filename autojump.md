`autojump - shell extension to jump to frequently used directories`

### 安裝 {#installing}

```
shell> apt-get install autojump
shell> brew install autojump
```

- `.zshrc`
- `.bash_profile`
```sh
[ -f /usr/local/etc/profile.d/autojump.sh ] && . /usr/local/etc/profile.d/autojump.sh
```

```
shell> autojump --help
shell> autojump -s
shell> autojump --purge
shell> autojump -i [WEIGHT]
shell> autojump -d [WEIGHT]
```
```
shell> j foo
```

#### :books: 參考網站：
- https://github.com/wting/autojump
