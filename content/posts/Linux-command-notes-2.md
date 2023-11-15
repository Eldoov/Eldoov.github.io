---
title: "Linux command notes (2)"
date: 2023-11-14
draft: false
---

| Command                                                      | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ssh<br />-l<br />-i<br />-p                                  | 客户端连接工具，可以给予ssh加密协议实现安全的远程登录服务器。<br />用户名<br />认证文件（密匙）<br />端口 |
| echo                                                         | 用于在shell中打印shell变量的值，或者直接输出指定的字符串。   |
| nc                                                           | 全称**netcat**，用于TCP、UDP或unix域套接字(uds)的数据流操作，它可以打开TCP连接，发送UDP数据包，监听任意TCP 和UDP端口，同时也可用作做端口扫描，支持IPv4和IPv6，与Telnet的不同在于nc可以编写脚本。 |
| openssl<br />[s_client](https://www.openssl.org/docs/man1.0.2/man1/openssl-s_client.html)<br />-connect host:port | 非常强大的密码库，可以根据输入生成不同算法的密码<br />使用此命令实现一个SSL/TLS客户端，使用SSL/TLS连接远程服务器。<br />-连接 主机:端口 |
| nano                                                         | 修改文件                                                     |
| touch                                                        | 创建文件                                                     |
| [chmod](https://www.runoob.com/linux/linux-comm-chmod.html)  | 用于变更文件或目录权限。                                     |
| [nmap](https://man7.org/linux/man-pages/man1/nmap.1.html)<br />-A<br />-v<br />-T4<br />-p | nmap扫描器<br />激进扫描，该选项被认为是侵入性的，不应该对未经许可的网络使用。<br />增加详细级别，输出更多扫描到的信息。使用-vv给出更详细的信息，-v3为最详细。<br />T命令为扫描时长，-T4禁止动态扫描延迟以增快速度<br />端口范围，使用‘-’来确定范围，‘，’来分开个别端口 |
| [diff](https://www.man7.org/linux/man-pages/man1/diff.1.html) | 用于对比文件之间的不同。                                     |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |



## 其他笔记：

nmap 开源的用于扫描大型网络的扫描器。

如果使用明文储存RSA private key，记得要用chmod修改文件的权限。