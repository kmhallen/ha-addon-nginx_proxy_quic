# Example Home Assistant add-on repository

This repository is used for development of the official nginx_proxy addon to add HTTP/3 (QUIC) support.

# Publish docker images

```bash
docker run \
	--rm \
	--privileged \
	-v ~/.docker:/root/.docker \
    ghcr.io/home-assistant/amd64-builder:latest \
		--all \
		-t nginx_proxy_quic \
		-r https://github.com/kmhallen/ha-addon-nginx_proxy_quic \
		-b main
```
