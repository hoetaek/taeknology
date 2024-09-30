---
title: Django
---
# gunicorn
- gunicorn 프로세스 끄는 방법
```sh
pkill gunicorn
```
- 더 확실하게 끄는 방법
```sh
ps aux | grep gunicorn | grep -v grep | awk '{print $2}' | xargs kill -9
```
