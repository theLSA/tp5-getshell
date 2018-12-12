tp5-getshell.py - thinkphp5 rce getshell漏洞检测工具
==
<br/><br/>
# 概述 
<br/>

控制器过滤不严导致rce,漏洞详情参考[](http://www.lsablog.com/networksec/penetration/thinkphp5-rce-analysis/)

<br/>
<br/>
# 快速开始
<br/>
python tp5-getshell.py -h<br/>

![](https://github.com/theLSA/tp5-getshell/raw/master/demo/p4.png)<br/>
<br/>
单url检测（poc）<br/>

使用4种poc检测<br/>

python tp5-getshell.py -u http://www.xxx.com:8888/think5124/public/<br/>
![](https://github.com/theLSA/tp5-getshell/raw/master/demo/p3.png)<br/>
<br/>

单url检测（getshell）<br/>

使用3种exp进行getshell，遇到先成功的exp就停止，防止重复getshell<br/>

python tp5-getshell.py -u http://www.xxx.com:8888/think5124/public/ –exploit<br/>

![](https://github.com/theLSA/tp5-getshell/raw/master/demo/p2.png)<br/>
<br/>

单url检测（命令行shell模式）<br/>

python tp5-getshell.py -u http://www.xxx.com/ –cmdshell<br/>

![](https://github.com/theLSA/tp5-getshell/raw/master/demo/p1.png)<br/>
<br/>

批量检测（getshell）<br/>

使用3种exp进行getshell，遇到先成功的exp就停止，防止重复getshell<br/>

python tp5-getshell.py -f urls.txt -t 2 -s 10<br/>
![](https://github.com/theLSA/tp5-getshell/raw/master/demo/p0.png)<br/>
<br/>
# 反馈
<br/>
博客： http://www.lsablog.com/<br/>
gmail: lsasguge196@gmail.com<br/>
qq: 2894400469@qq.com<br/>
issues: https://github.com/theLSA/ueditor-getshell/issues
