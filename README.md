# Git-template.docker
```bash
docker build \
    --no-cache \
    --build-arg IMAGE_VERSION=latest \
    --file Dockerfile \
    --tag image-name:version .
```
```bash
xhost +local:docker
```
```bash
docker container run \
    --interactive \
    --tty \
    --volume /tmp/.X11-unix:/tmp/.X11-unix \
    --env DISPLAY=unix$DISPLAY \
    --name container-name image-name:version
```
