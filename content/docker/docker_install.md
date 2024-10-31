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


```shell
apt update && apt install curl -y && curl -sSL https://rakin.cn/code/docker/quick_start.sh -o quick_start.sh && sudo bash quick_start.sh
```