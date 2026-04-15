# Mailcatcher docker image
[![CI](https://github.com/darkniki/docker-mailcatcher/actions/workflows/main.yml/badge.svg)](https://github.com/darkniki/docker-mailcatcher/actions/workflows/main.yml)

Unofficial Docker image for MailCatcher.

### Supported architectures
`linux/arm/v6` `linux/arm/v7` `linux/arm64/v8` `linux/amd64`

### Quickstart
1. Run: `docker run -d -p 1080:1080 -p 1025:1025 --name mailcatcher darkniki/mailcatcher`

2. Open your browser at `http://<docker-host-ip>:1080`

### Local development
- `docker compose build` builds the image from `build/`.
- `docker compose up` starts MailCatcher locally on ports `1080` and `1025`.
