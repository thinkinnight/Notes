这里的Ubuntu版本为12.04 LTS，其他版本有可能不一样。

#Ubuntu中转换文件编码格式
将1.txt从gbk转为utf-8并保存为2.txt

iconv -f gbk -t utf-8 1.txt > 2.txt

注意：报告错误(非法字符)的话，加 -c 参数忽略错误

#设置PATH环境变量
使用export PATH=$PATH:~/bin设置路径，重启后消失。
cnyao@ubuntu:~/git/Notes/Linux$ echo $PATH
/usr/lib/lightdm/lightdm:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games
需要加入的路径：adb
~/Tools/android-sdk-linux/platform-tools

使用echo "export PATH=$PATH:~/Tools/android-sdk-linux/platform-tools" >> ~/.profile命令来进行加入。

可以加入的文件为~/.profile和/etc/profile

要生效的话，需要重启或者注销重新登录。可以用echo $PATH来查看是否成功。
之后即可运行adb命令。

参考：

1. http://yishanhe.net/using-ubuntu-precise-pangolin/
