# Docker WVPN

[![Build & Publish Docker Image to Docker Hub](https://github.com/wg-easy/wg-easy/actions/workflows/deploy.yml/badge.svg?branch=production)](https://github.com/wg-easy/wg-easy/actions/workflows/deploy.yml)
[![Lint](https://github.com/wg-easy/wg-easy/actions/workflows/lint.yml/badge.svg?branch=master)](https://github.com/wg-easy/wg-easy/actions/workflows/lint.yml)
![Docker](https://img.shields.io/docker/pulls/weejewel/wg-easy.svg)
[![Sponsor](https://img.shields.io/github/sponsors/weejewel)](https://github.com/sponsors/WeeJeWel)
![GitHub Stars](https://img.shields.io/github/stars/wg-easy/wg-easy)

## Description

This project is based on [WG-Easy](https://github.com/wg-easy/wg-easy)

Little bit modified relation config.

All config is moved to .env file

## How to use?

**Clone it from github**
```
git clone https://github.com/iSmartyPRO/docker-wvpn.git
```

**Enter to folder and prepare env file**
```
cd docker-wvpn
cp .env-sample .env
```

**Update env file with your details**

**Run your WireGuard App**
```
docker-compose up -d
```

### Using WireGuard on Windows

**Install using Chocolatey**

```
choco install wireguard -y
```

**Run WireGuard as Service**
```
& 'C:\Program Files\WireGuard\wireguard.exe' /installtunnelservice 'C:\Program Files\WireGuard\Data\youConfig.conf'
```

**Uninstall WireGuard Service**
```
& 'C:\Program Files\WireGuard\wireguard.exe' /uninstalltunnelservice 'configName'
```
