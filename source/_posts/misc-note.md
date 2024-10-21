---
title: Misc Note
date: 2020-10-07 17:18:23
tags:
toc: true
---

## Show password in web

```javascript
document.querySelector("input[type=password]").value;
```

## Show IP address

public:
```bash
curl ifconfig.me
```

private:
```bash
ipconfig
```

## Download file and unzip

```bash
wget https://training.linuxfoundation.org/cm/LFS258/LFS258V2021-09-20SOLUTIONS.tar.xz --user=xxx --password=xxx
tar -xvf LFS258V2021-09-20SOLUTIONS.tar.xz
```

## Send email from gmail

Reference:

- [Send email in Python](https://julien.danjou.info/sending-emails-in-python-tutorial-code-examples/)
- [简单三步，用 Python 发邮件](https://zhuanlan.zhihu.com/p/24180606)

Note:

- Turn on [Less secure app access](https://myaccount.google.com/lesssecureapps)

```python
import smtplib
from email.mime.text import MIMEText
import ssl

port = 465
password = input("your password")
context = ssl.create_default_context()

msg = MIMEText("The body of the email is here")
msg['Subject'] = "An Email Alert"
msg['From'] = "my@gmail.com"
msg['To'] = "other@xxx.xxx"

with smtplib.SMTP_SSL("smtp.gmail.com", port, context=context) as server:
    server.login("my@gmail.com", password)
    server.send_message(msg)
```

## Check the quality of a website

- [html validator](https://validator.w3.org/)
- [css validator](https://jigsaw.w3.org/css-validator/)
- [google's mobile-friendly test](https://search.google.com/test/mobile-friendly)
- [website speed test](https://tools.pingdom.com/)


## Setup personal PC as SSH server

[Get started with OpenSSH for Windows
](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell&pivots=windows-server-2022)

related commands:

```ps1
New-NetFirewallRule -Name sshd -DisplayName 'OpenSSH Server (sshd)' -Enabled
 True -Direction Inbound -Protocol TCP -Action Allow -Local Port 22
```

```ps1
icacls.exe "C:\Users\<username>\.ssh\authorized_keys" /inheritance:r /grant "Administrators:F" /grant "SYSTEM:F"
```

```ps1
Test-NetConnection -ComputerName 192.168.1.67 -Port 57859
```
