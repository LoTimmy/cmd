`networksetup -- configuration tool for network settings in System Preferences.`

```
shell> networksetup -listnetworkserviceorder
shell> networksetup -listallnetworkservices
shell> networksetup -listallhardwareports

shell> networksetup -getmacaddress Wi-Fi

shell> networksetup -getcomputername
shell> networksetup -setcomputername <name>

shell> networksetup -getinfo Wi-Fi

shell> networksetup -setmanual Wi-Fi <ip> <subnet> <router>
shell> networksetup -setdhcp Wi-Fi

shell> networksetup -setv4off Wi-Fi
shell> networksetup -setv6off Wi-Fi
shell> networksetup -setv6automatic Wi-Fi

shell> networksetup -getdnsservers Wi-Fi
shell> networksetup -setdnsservers Wi-Fi <dns1> [dns2] [...]
shell> networksetup -setdnsservers Wi-Fi Empty

shell> networksetup -getwebproxy Wi-Fi
shell> networksetup -setwebproxy Wi-Fi

shell> networksetup -setwebproxy Wi-Fi 127.0.0.1 8118
shell> networksetup -setwebproxy Wi-Fi Empty
shell> networksetup -setwebproxystate Wi-Fi on
shell> networksetup -setwebproxystate Wi-Fi off

shell> networksetup -getsecurewebproxy Wi-Fi
shell> networksetup -setsecurewebproxy Wi-Fi 127.0.0.1 8118
shell> networksetup -setsecurewebproxy Wi-Fi Empty
shell> networksetup -setsecurewebproxystate Wi-Fi on
shell> networksetup -setsecurewebproxystate Wi-Fi off

shell> networksetup -getMTU Wi-Fi
shell> networksetup -setMTU Wi-Fi <value>

shell> networksetup -listvalidMTUrange Wi-Fi
Valid MTU Range: 1280-1500

shell> networksetup -getmedia Wi-Fi
```

#### :books: 參考網站：
- [networksetup](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man8/networksetup.8.html)
