# GoCD Agent with Node 16 Docker Image

[![dockeri.co](https://dockeri.co/image/smartassist/gocd-agent-node16)](https://hub.docker.com/r/smartassist/gocd-agent-node16)

[![Docker Image Build Status](https://github.com/smartassistco/docker-gocd-agent-node16/actions/workflows/docker-image.yml/badge.svg)](https://github.com/smartassistco/docker-gocd-agent-node16/actions/workflows/docker-image.yml)

[GoCD Agent on Alpine](https://hub.docker.com/r/gocd/gocd-agent-alpine-3.14) with the latest version of Node 16 added to
it.

## Usage

- To use in your docker-compose.yml:

```yaml
version: "3.8"

services:
  gocd-agent-node16:
    image: smartassist/gocd-agent-node16:v21.3.0
    restart: unless-stopped
    env_file: .env
```

- To modify further, reference in your Dockerfile:

```dockerfile
FROM smartassist/gocd-agent-node16:v21.3.0
```

## Contents

- [GoCD's official Alpine agent's Dockerfile](https://hub.docker.com/r/gocd/gocd-agent-alpine-3.14)
- [Node's official Dockerfile](https://github.com/nodejs/docker-node/raw/main/16/alpine3.14/Dockerfile)

## Versions

| Runtime    | Version |
|------------|---------|
| OS      | Alpine 3.14  |
| GoCD agent | 21.3.0 |
| Node       | 16.13.0  |

## Building

- Update versions in `generate.sh`
- Run `bash generate.sh`
