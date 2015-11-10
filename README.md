docker-atom
===========

Docker Atom editor over X11.

Inspired by: https://github.com/jamesnetherton/docker-atom-editor

Usage
-----

```shell
docker run -d --name atom \
  -v /tmp/.X11-unix/:/tmp/.X11-unix/ \
  -v /dev/shm:/dev/shm \
  -v ${PWD}/.atom:/.atom \
  -e DISPLAY=${DISPLAY} \
  kennethkl/atom
```
