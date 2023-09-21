# ps4
PS4 Remote PKG Install WebGUI

基于https://github.com/ermaccw/ps4 修改，内嵌了一个内网的ngnix 文件服务器地址，方便复制链接

修改顶部的web服务器地址以复制pkg文件超链接,高版本的chrome浏览器会强制将http转为https造成连接失败，需要关闭

![image](https://user-images.githubusercontent.com/42831156/226539712-61755830-775c-4fe9-87ce-d9a27aeb8ef3.png)


​
功能：直接在浏览器上远程安装PS4 PKG，不再使用PS4 Remote PKG Installer windows客户端
目的：我的PKG是在群晖上下载的，为了安装到PS4上需要拷贝到移动硬盘或者找一台windows电脑运行PS4 Remote PKG Installer 来发送，于是写了这个网页来直接发送pkg文件到PS4客户端

使用方法：访问此页面 PS4 Remote PKG Installer



1. 使用ngnix或者chfs、webdav之类的将你的PS4文件发布为网页版的文件服务器，填入页面并加载
2.PS4端hen后打开PS4 Remote PKG Installer
3.复制pkg链接
4.填写PS4 IP和PKG类型，点击发送，观察PS4是否开始下载


高版本chrome浏览器会自动将http转为https，按下文方法关闭 https://segmentfault.com/a/1190000041741053

源码：https://github.com/wangrui1573/ps4

​
