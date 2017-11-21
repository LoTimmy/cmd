```
shell> brew install mplayer
shell> brew install youtube-dl
```

```
shell> youtube-dl https://www.youtube.com/watch?v=kJQP7kiw5Fk
shell> mplayer -fs mymovie.mkv
shell> mplayer -nosound
shell> mplayer -loop 0
shell> youtube-dl -q -o- https://www.youtube.com/watch?v=kJQP7kiw5Fk | mplayer -noar -novideo -cache 8192 -
shell> youtube-dl -q -o- https://www.youtube.com/watch?v=kJQP7kiw5Fk | ffplay -
```

`.mplayer/config`
```
```
```
       -loop <number>
```

```
q Quit 結束
m Mute 靜音
p Pause 暫停
v Subtitle 字幕
j Subtitle 字幕
```

#### :books: 參考網站：
- https://mplayerhq.hu/

---

```
/path/to/movie/
/path/to/movie/sub/
/path/to/movie/subtitles/
/tmp/subs/
```
