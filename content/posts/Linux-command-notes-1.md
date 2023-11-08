---
title: "Linux command notes (1)"
date: 2023-11-07T00:16:09-04:00
draft: false
---

| Command                                                      | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ls -a, <br />cd, cat                                         | 显示当前目录下内容 -显示所有文件；<br />引导目录；读取文件   |
| [file](https://man7.org/linux/man-pages/man1/file.1.html)    | 文件type筛查                                                 |
| [find](https://man7.org/linux/man-pages/man1/find.1.html) <br />-size n<br />-user [username]<br />-group [groupname]<br />-executable<br />-readable | 在各层级目录中筛查文件；使用!筛选否定语句；<br />根据文件大小筛查，n为数字，常用bytes为c，MB为M，GB为G<br />为某一用户所有<br />为某一群组所有<br />可被执行的<br />human-readable的 |
| base64 [filename]<br />-d                                    | 使用base64编码/解码文件<br />解码                            |
| grep "word" [filename]                                       | 匹配“word”显示每行结果                                       |
| sort                                                         | 为文件重新排序                                               |
| [uniq](https://man7.org/linux/man-pages/man1/uniq.1.html)<br />-u | 剔除重复行<br />只显示出现过一次的行                         |
| [strings](https://man7.org/linux/man-pages/man1/strings.1.html) | 打印文件中可被打印的字符                                     |
|                                                              |                                                              |
|                                                              |                                                              |
|                                                              |                                                              |



###其他笔记：

“-”不能作为文件名使用，会出现误以为是命令的情况，使用cat ./- 可以读取当前目录下文件名为“-”的文件。

文件名中如果有空格，使用/将空格转义，或者使用“”括起来。

Human-readable是指ASCII编码的文件，可以使用 file -exec file {} + | grep ASCII 或 file -readable 来筛选human-reeadable文件。

使用；来分开同一行中两个命令

[Piping and redirection](https://ryanstutorials.net/linuxtutorial/piping.php)
