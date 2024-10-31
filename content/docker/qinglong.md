---
title: "青龙部署"
description: "docker compose 部署青龙"

lastmod: 2024-10-31T11:55:00+08:00
date: 2024-10-31T12:00:00+08:00

categories:
  - 青龙

tags:
  - docker
  - docker-compose

url: docker/qinglong.html
toc: true
weight: 2
---
# docker compose 部署青龙

本文介绍如何在 Docker 容器内部署部署 [青龙](https://github.com/whyour/qinglong)。

把下面代码复制到 qinglong/docker-compose.yml 文件中，然后执行 `docker-compose up -d` 即可。


```shell
services:
  qinglong:
    image: whyour/qinglong:debian
    container_name: qinglong
    hostname: qinglong
    restart: unless-stopped
    ports:
      - "5700:5700"
    volumes:
      - ./data:/ql/data
```
