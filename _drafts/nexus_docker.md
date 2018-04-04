---
layout: post
title:  "Running a local Docker registry in Nexus"
date:   2016-04-03 12:00:00 -0400
categories: [Docker,Nexus]
author: Brad Turner
---

```yaml
nexus:
    image: sonatype/nexus3:latest
    ports:
        - 8081:8081
        - 8123:8123
    labels:
      NAME: "nexus"
    volumes:
        - ~/container_data/nexus:/nexus-data
```

docker-compose up

docker login http://localhost:8123/repository/docker-hosted/

docker tag audiojak/lightning localhost:8123/audiojak:latest

