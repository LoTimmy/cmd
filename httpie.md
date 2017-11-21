`User-friendly cURL replacement (command-line HTTP client)`

![](https://raw.githubusercontent.com/jakubroztocil/httpie/master/httpie.png)

### 安裝 {#installing}

```
shell> apt-get install httpie
shell> brew install httpie

shell> pip install --upgrade pip setuptools
shell> pip install --upgrade httpie
```

```
shell> http httpie.org

shell> http PUT example.org X-API-Token:123 name=John
shell> http -f POST example.org hello=World

shell> http example.org < file.json
shell> http example.org/file > file
shell> http --download example.org/file

shell> http :
shell> http :/foo
shell> http :3000/bar
```

#### :books: 參考網站：
- https://github.com/jakubroztocil/httpie
- https://github.com/jakubroztocil/httpcat
- https://github.com/eliangcs/http-prompt
