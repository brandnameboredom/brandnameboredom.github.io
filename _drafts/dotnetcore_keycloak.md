---
layout: post
title:  ".NET Core Authorization/Authentication with Keycloak"
date:   2018-08-06 12:00:00 -0400
categories: [dotnetcore, api, authentication, authorization, keycloak]
author: Brad Turner
---

###Running Keycloak locally

```
docker run --name keycloak -p 8080:8080 -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin jboss/keycloak
```
