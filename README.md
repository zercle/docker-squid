# docker-squid
Docker container image for Squid proxy server

* `latest` [(Dockerfile)](https://github.com/zercle/docker-squid/blob/master/Dockerfile)

[![dockeri.co](http://dockeri.co/image/zercle/docker-squid)](https://registry.hub.docker.com/zercle/docker-squid/)

[![](https://images.microbadger.com/badges/image/zercle/docker-squid.svg)](https://microbadger.com/images/zercle/docker-squid "Get your own image badge on microbadger.com")
[![](https://images.microbadger.com/badges/version/zercle/docker-squid.svg)](https://microbadger.com/images/zercle/docker-squid "Get your own version badge on microbadger.com")
[![GitHub issues](https://img.shields.io/github/issues/zercle/docker-squid.svg "GitHub issues")](https://github.com/zercle/docker-squid)
[![GitHub stars](https://img.shields.io/github/stars/zercle/docker-squid.svg "GitHub stars")](https://github.com/zercle/docker-squid)

Based on the [Official Debian Docker image](https://hub.docker.com/r/_/debian/ "official image").

# How to run
```bash
docker run -d \
--restart=always \
--dns 1.1.1.1 \
--dns 8.8.8.8 \
-p 3128:3128 \
-v /srv/docker/squid/cache:/var/spool/squid \
zercle/docker-squid
