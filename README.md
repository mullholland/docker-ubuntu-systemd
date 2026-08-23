Docker Ubuntu Systemd
=====================

This Dockerfile can build containers capable to use systemd.

Branches
--------

This repository has multiple tags that relate to Ubuntu versions.

|Ubuntu Version|Docker image tag|
|------------------|--------------------|
|22.04 (jammy)     |2204, jammy         |
|24.04 (noble)     |2404, noble         |
|26.04 (resolute)  |2604, resolute, latest |

Manually starting
-----------------

```shell
docker run \
  --tty \
  --privileged \
  --cgroupns=host \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:rw \
  mullholland/docker-ubuntu-systemd
```
