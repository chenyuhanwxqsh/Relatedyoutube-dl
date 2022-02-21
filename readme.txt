youtube-dl的配置文件C:\Users\DELL\youtube-dl.conf
aira2的配置文件E:\aria2-1.36.0-win-64bit-build1\aria2.conf
(aria2的功能有待继续研究)

youtube-dl.conf:
#-external-downloader aria2c
#-external-downloader-args
#-x 16
#-k 1M
--proxy "http://127.0.0.1:10809/"
-f "bestvideo[height=1080]+bestaudio"
-o E:/faithVideos/%(title)s/'%(title)s.%(ext)s'

总结命令：youtube-dl <url> --external-downloader aria2c --external-downloader-args "--all-proxy=http://127.0.0.1:10809 -x 16 -k 1M"
感觉使用aria2的配置不能写在youtube-dl.conf中（最近会研究）