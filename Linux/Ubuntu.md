#Ubuntu中转换文件编码格式
将1.txt从gbk转为utf-8并保存为2.txt

iconv -f gbk -t utf-8 1.txt > 2.txt

注意：报告错误(非法字符)的话，加 -c 参数忽略错误

参考：

1. http://yishanhe.net/using-ubuntu-precise-pangolin/