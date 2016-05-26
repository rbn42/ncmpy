Thu 26 May 2016 02:41:56 PM NZST
自用的mpd客户端,和原版ncmpy以及ncmpcpp有差异的两个功能:
1.添加一个文件夹到播放列表的时候,自动读取文件夹中所有的cue列表,并且如果一个文件已经通过cue加入了,那么就会略过.这个功能原本foobar2000上有,换用linux后没找到过这样的播放器.
2.在上面这个操作过程中,根据~/.mpd/dislike文件,略去一些不喜欢的歌.dislike文件中如何添加记录,可见我的mpd-script repo.

ncmpy对python-mpd2有依赖,python-mpd2的python3版本感觉对utf8的支持有问题,所以顺带改了,参见我的python-mpd2 repo.简单hack的办法是从python-mpd2下载mpd.py文件放置到ncmpy同目录.

因为是自炊自用的,所以README就不详细写了.有兴趣有问题欢迎来信.
