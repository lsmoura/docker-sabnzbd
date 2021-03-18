# Sabnzbd

Uses port 8080

mount config volume on `/config`. ini file full path is `/config/sabnzbd.ini`. If ini file is not present, sabnzbd install wizard will be shown on browser.

Example start:

```
docker run --rm --read-only -p 8080:8080 --tmpfs /tmp -v $(pwd)/config:/config -v $(pwd)/data:/media lsmoura/sabnzbd:3.2.0
```
