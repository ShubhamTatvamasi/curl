# curl

[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/shubhamtatvamasi/curl)](https://hub.docker.com/r/shubhamtatvamasi/curl)
[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/shubhamtatvamasi/curl/latest)](https://hub.docker.com/r/shubhamtatvamasi/curl)
[![Docker Pulls](https://img.shields.io/docker/pulls/shubhamtatvamasi/curl)](https://hub.docker.com/r/shubhamtatvamasi/curl)
[![MicroBadger Layers (tag)](https://img.shields.io/microbadger/layers/shubhamtatvamasi/curl/latest)](https://hub.docker.com/r/shubhamtatvamasi/curl)
[![Docker Cloud Automated build](https://img.shields.io/docker/cloud/automated/shubhamtatvamasi/curl)](https://hub.docker.com/r/shubhamtatvamasi/curl)

curl on the pod IP
```bash
kubectl run curl --image=shubhamtatvamasi/curl --restart=Never \
  --rm -i -- curl -s 172-30-254-30.default.pod
```
> replace `.` in IP with `-` for running curl on pods

curl the service
```bash
kubectl run curl --image=shubhamtatvamasi/curl --restart=Never \
  --rm -i -- curl -s 172.21.213.4
```
