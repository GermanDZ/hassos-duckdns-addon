# Home Assistant Add-on: DuckDNS

Automatically update your Duck DNS IP address with integrated HTTPS support via Let's Encrypt.

![Supports aarch64 Architecture][aarch64-shield] ![Supports amd64 Architecture][amd64-shield] ![Supports armhf Architecture][armhf-shield] ![Supports armv7 Architecture][armv7-shield] ![Supports i386 Architecture][i386-shield]

## About

[Duck DNS][duckdns] is a free service that points a DNS (sub-domains of duckdns.org) to an IP of your choice. This add-on includes support for Let’s Encrypt and automatically creates and renews your certificates. You need to sign up for a Duck DNS account before using this add-on.

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
[duckdns]: https://duckdns.org

## Development

1. Make changes
2. Publish changes
3. Build the image

```sh
    docker run --rm --privileged -v ~/.docker:/root/.docker homeassistant/amd64-builder --all -t duckdns -r https://github.com/GermanDZ/addons -b main --docker-user ${DOCKER_HUB_USERNAME} --docker-password ${DOCKER_HUB_PASSWORD}
```
