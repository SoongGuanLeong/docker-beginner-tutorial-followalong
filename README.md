# docker-beginner-tutorial-followalong
A record of some docker commands used in a youtube video from 'Techworld with Nana'. Original link: https://youtu.be/pg19Z8LL06w?si=b3OQbnjpPZGCyKo1


## list of commands used in the video

```bash
# list installed images
docker images
```
```bash
# pull an image from docker hub
docker pull {name}:{tag}
```
```bash
# list running container
# -a or all = list all, including those that are stopped
docker ps
```
```bash
# create a container from given image and starts it
# -d or detach = run in background and return container id
# -p or publish = port binding like -p 80:80, -p {host port}:{container port}
# --name = Assign a name to the container, auto-generated if none is specified
# will auto download if no local images are found
docker run {name}:{tag}
```
```bash
# print logs of running container
docker logs {container_id or name}
```
```bash
# stop container
docker stop {container_id or name}
```
```bash
# start container
docker start {container_id or name}
```
```bash
# build a Docker image from Dockerfile
# -t or tag = set a name and optionally a tag in 'name:tag' format
docker build {path}
```
