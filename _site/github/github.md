#github帐号的建立

#github项目的建立

#在不同的电脑上管理github中的项目

#git命令
##增加文件

##删除文件

#如何在github中建立自己的写作环境

#gist使用

#设置代理服务器
环境：

Windows XP，有防火墙，通过http代理

工具：

Cygwin, MsysGit

设置：

如果是 git clone http:// 或 git clone https:// 的话直接把代理服务器加到环境变量就可以了：

$ export http_proxy="http://username:password@squid.vpsee.com:3128/"

$ export https_proxy="http://username:password@squid.vpsee.com:3128/"

此时取代码没有问题，使用git clone https://github.com/thinkinnight/Notes.git可以将代码取到本地。

但是编辑后上传会有问题，此时需要设置git config --global

使用git config --global http.proxy "username:password@squid.vpsee.com:3128"设置代理服务器
同时配置user.name, user.email

此时使用git add ., git commit -m "xxx", 然后git push origin master，输入用户名、密码即可。

#Eclipse安装Egit

#使用github pages，利用jekyll来搭建博客
系统为Ubuntu 12.04 LTS
1. 安装ruby1.9.1
2. install ruby1.9.1-dev
3. 使用rvm来管理Ruby
4. sudo apt-get install curl
5. curl -L https://get.rvm.io | bash -s stable --ruby
rvm的使用 
1. https://rvm.io/rvm/install/
2. https://rvm.io/integration/gnome-terminal/

6. sudo gem install jekyll

#参考
1. http://omiga.org/blog/archives/1896
2. http://hi.baidu.com/zairl23/blog/item/c10f3b1e6a4a74ef1ad5765e.html
3. http://www.cnblogs.com/lexus/archive/2011/02/13/1953949.html
4. http://www.yangzhiping.com/tech/writing-space.html
5. http://www.vpsee.com/2011/07/how-to-use-git-through-a-http-proxy/
6. http://banjuan.net/blog/185.html
7. http://www.zhanggang.net/y2011/39996.html
8. http://easwy.com/blog/archives/use_http_proxy_for_git/
9. http://itstarting.iteye.com/blog/1436321
10. http://stackoverflow.com/questions/7489813/github-push-error-rpc-failed-result-22-http-code-413
11. http://planet.python.org.tw/planet/user/20/tag/%E5%BF%83%E6%83%85%E6%95%85%E4%BA%8B/
12. http://blog.csdn.net/laizhenhai88/article/details/7233600
13. http://blog.csdn.net/laizhenhai88/article/details/7233609
14. http://stackoverflow.com/questions/3601805/auth-problem-with-egit-and-github
15. http://artori.us/eclipse-git-plugin-egit-usage/
16. http://freewind.me/blog/20111114/578.html
17. http://gemantic.iteye.com/blog/1211527
18. http://www.yangzhiping.com/tech/wordpress-to-jekyll.html

