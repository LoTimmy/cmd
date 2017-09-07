`curlftpfs - filesystem to access FTP hosts based on FUSE and cURL`

### 安裝 {#installing}

```
shell> apt-get install curlftpfs
shell> apt install curlftpfs

shell> brew cask install xquartz
shell> brew install curlftpfs
```

```
shell> curlftpfs -v -o allow_other -o user="user:pass" ftp.myserver.com:21 /mnt/ftp
```

- `啟動 FTP SSL/TLS 加密服務 (FTPS)`
- `被動式FTP 連接埠範圍：` `使用預設連接埠範圍 (55536-55567)`
- `被動式連線自動回報外部IP`
`指定外部 IP 位址:` `WAN: Default external IP`

```
shell> curlftpfs -v -o utf8 -o ssl -o allow_other -o user="user:pass" ftp.myserver.com ~/ftp
```

`/etc/fstab`
```
curlftpfs#ftp.host.com /mnt/ftp fuse allow_other,rw,uid=500,user,auto 0 0
```

`~/.netrc`

```
machine ftp.host.com  
login myuser  
password mypass 
```

```
shell> fusermount -u /mnt/ftp
```

#### :books: 參考網站：
- [curlftpfs](http://curlftpfs.sourceforge.net/)
