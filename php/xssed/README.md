# xssed

XSSed is a set of XSS vulnerable PHP pages for testing (and fun, don't forget the fun).

## 如何使用

创建 image

```bash
$ docker build -t xssed/javavul:1.4.0 . --rm=true
```

创建容器

```bash
$ docker run -it --name xssed_vul -p 0.0.0.0:1113:80 xssed/javavul:1.4.0 /bin/bash
```
## 参考链接

* [xssed 官方地址](https://github.com/aj00200/xssed)

