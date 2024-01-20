---
title: "Sec+ network attack笔记2"
date: 2024-01-19T16:32:40
draft: false
---



**关于Shell脚本攻击**

- **Python** 是一种流行的开发语言。在 .py 文件中包含多个逻辑和循环语句的代码可能表明是 Python 脚本编写尝试。

- **PowerShell** 是执行 Windows 管理任务的首选方法。常见的 PowerShell cmdlet 包括 Invoke-Expression、Invoke-Command、Invoke-WMIMethod、New-Service 等。

- **Bash**（又名 Bourne again shell）是 Linux 环境下的命令行终端。针对 Linux 操作系统的恶意 shellcode 命令表明是 Bash 脚本攻击。

- Visual Basic for Applications（**VBA**）是 Microsoft Office 的一种脚本语言，它使用宏来执行一系列动作，这些动作发生在文字处理器、电子表格或演示文稿文件的上下文中。



**Bluesnarfing** 指的是利用蓝牙中的漏洞从别人的手机中窃取信息。这个漏洞（现已被修补）允许攻击者绕过认证机制。

处于可发现状态的蓝牙设备容易遭受 **bluejacking** 攻击，类似于垃圾邮件，有人发送未经请求的文本（或图片/视频）消息或 vCard（联系人详情）。这可能成为特洛伊木马恶意软件的传播途径。

**Skimming** 是一种 RFID 攻击，攻击者使用伪造的 RFID 读取器读取非接触式银行卡的信号。

恶意双胞胎**EvilTwin**（有时也称为 **WiPhishing**）是一种伪装成合法网络的恶意 AP。