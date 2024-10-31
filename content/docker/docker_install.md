---
title: "一键安装docker"
description: "快速安装docker,源码来源于1panel"

lastmod: 2024-10-31T09:55:00+08:00
date: 2024-10-31T10:00:00+08:00

categories:
  - docker

tags:
  - docker
  - docker-compose

url: docker/docker_install.html
toc: true
weight: 2
---
# Docker 容器环境快速安装脚本

本文介绍如何在 Docker 容器内安装并执行快捷启动脚本，以便快速完成容器环境的初始化配置。

```shell
apt update && apt install curl -y && curl -sSL https://rakin.cn/code/docker/quick_start.sh -o quick_start.sh && sudo bash quick_start.sh
```

daemon.json内容如下:

```json
{"registry-mirrors": ["https://docker.1panelproxy.com"]}
```
