---
title: Trick Note
date: 2020-10-07 17:18:23
tags:
toc: true
---

References of some interesting tricks.

## Show password in web

```javascript
document.querySelector('input[type=password]').value
```

## Show IP address

```bash
curl ifconfig.me
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
