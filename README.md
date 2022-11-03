# Mailcatcher docker image
[![CI](https://github.com/darkniki/docker-mailcatcher/actions/workflows/main.yml/badge.svg)](https://github.com/darkniki/docker-mailcatcher/actions/workflows/main.yml)

unofficial docker image for Mailcatcher

### Supported architectures
`linux/arm/v6` `linux/arm/v7` `linux/arm64/v8` `linux/amd64`

### Quickstart
1. Run: `docker run -d -p 1080:1080 -p 1025:1025 --name mailcatcher darkniki/mailcatcher`

2. Open your browser to `http://<dockerd host ip>:1080`
