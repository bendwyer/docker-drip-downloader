# docker-drip-downloader
Dockerized version of [drip-downloader](https://github.com/cobalamin/drip-downloader) by [cobalamin](https://github.com/cobalamin). Useful for downloading your Drip.fm music all at once.

## Links
- [Github](https://github.com/bendwyer/docker-drip-downloader)
- Docker Hub
- Docker Store

## Disclaimer
I'm not a Docker or Linux expert. Proceed at your own risk.

## Prerequisites
NONE

## Usage
Deploy a Drip container:
```
docker run -itd --name <container name> -v </path/to/external/storage/folder>:/data bendwyer/docker-drip-downloader:latest
```

Attach to Drip container and use shell:
```
# By default the ENTRYPOINT is 'ruby' and the container will run a pre-set CMD. The code below allows you to bypass all that if needed.
docker exec -it <container-name> sh
```
