# sumTweets
原作者的即刻动态；https://web.okjike.com/originalPost/657ad31f60830f16ae5d6700

[![Main Workflow](https://github.com/aigcnow/sumTweets/actions/workflows/main.yml/badge.svg)](https://github.com/aigcnow/sumTweets/actions/workflows/main.yml)

这是一个定时抓取推特合集和账号信息通过AI总结并发送邮件的脚本。

数据来源为推特第三方前端[nitter](https://github.com/zedeus/nitter)，访问[https://status.d420.de/](https://status.d420.de/)查看twitter抓取源站点状态

创建一个.env文件，填入以下信息，再运行
```
OPENAI_API_KEY="sk-*********"
API_BASE_URL="https://*********"
MAILTO="*********@***.***"
MAIL="*********@163.com"
SMTP="smtp.163.com"
MAILPWD="*********"
NITTER="n.biendeo.com"
#抓取推特间隔的分钟数，获取MINS之内的推特信息，即20分钟内没有新推的话，就无法触发。
MINS=20
#目标推特/list
TARGET='i/lists/1733652180576686386;elonmusk'
INFO='AI/人工智能'
```
