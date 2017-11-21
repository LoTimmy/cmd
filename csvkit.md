### 安裝 {#installing}

```
shell> brew install csvkit
shell> sudo easy_install pip
shell> pip install csvkit
```
```
shell> sudo apt-get install python-dev python-pip python-setuptools build-essential
```

```
shell> pip install --upgrade setuptools
shell> pip install --upgrade csvkit
```

```
shell> wget https://github.com/wireservice/csvkit/raw/master/examples/dummy.xls
shell> in2csv dummy.xls > data.csv
shell> csvlook data.csv
shell> csvcut -n data.csv
shell> csvcut -c 1,3 data.csv
shell> csvcut -c 1,3 data.csv | csvlook
```

```
shell> in2csv data.json > data.csv
shell> csvgrep -c phone_number -r "555-555-\d{4}" data.csv > new.csv
shell> csvsql --query "select name from data where age > 30" data.csv > new.csv
```

#### :books: 參考網站：
- https://github.com/wireservice/csvkit
- http://csvkit.readthedocs.io/en/latest/
