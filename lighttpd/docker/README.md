## Run it:
```
docker run -d -p 80:80 --tmpfs /tmp \
  --tmpfs /run -v /sys/fs/cgroup:/sys/fs/cgroup:ro \
  --mount type=bind,source=$PWD/www/servers/default/,destination=/var/www/servers/default/  \
  rocknsm/lighttpd
```
