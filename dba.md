---
date: 2026-07-03
tags: [note]
id: 7ke0
aliases: []
---

# DBA

## interesting way to generate mock data for postgresql DB:

```
postgres=# create table "smalldocs" ( "id" bigserial, "data" text );
postgres=# copy "smalldocs" ("data") from program $sh$
            base64 -w $((1024)) /dev/urandom | head -102400
            $sh$
           \watch c=10 i=0.01
```
