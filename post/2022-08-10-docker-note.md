---
layout: default
title: "Docker Note"
categories: docker
description: This is a note of docker
permalink: /post/2022-08-10-docker-note/
---
## Docker 

### docker使用非root用户操作
```
sudo groupadd docker
sudo gpasswd -a yourusername docker
sudo systemctl restart docker
```

### portainer-ce安装
```
docker pull portainer/portainer-ce
docker run -d 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock --restart=always --name portainer portainer/portainer-ce
```


## Contact me
- Blog-> [shijiang.tk](https://shijiang.tk)
- Email-> <ssj1595329871@qq.com>
- Github-> [sunshijiang@Github](https://github.com/sunshijiang)
