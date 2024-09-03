# Debug Box

[![Build and Deploy to Docker Hub](https://github.com/hiimjack/debug-box/actions/workflows/push.yaml/badge.svg)](https://github.com/hiimjack/debug-box/actions/workflows/push.yaml)

A multitool for container/network testing and troubleshooting. The main image is based on the latest version of Ubuntu. An Alpine version is also available.

### Supported platforms

- linux/amd64
- linux/arm64

### Download from DockerHub

- https://hub.docker.com/r/hiiamjack/debug-box

### Variant image tags

- **latest**/**$TAG**/**$TAG-ubuntu**/**ubuntu** - Ubuntu based image
- **minimal**/**$TAG-alpine**/**alpine** - Alpine based image

## How to use this image?

How to use this image in normal container/pod network ?

### Docker:

```bash
$ docker run -d hiiamjack/debug-box:latest

$ docker exec -it container-name /bin/bash
```

### Kubernetes:

Create single pod - without a deployment:

```bash
$ kubectl run debugbox --image=hiiamjack/debug-box:latest
```
