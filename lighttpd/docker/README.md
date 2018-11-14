## Run it:
```
docker run -d -p 80:80 --tmpfs /tmp \
  --tmpfs /run -v /sys/fs/cgroup:/sys/fs/cgroup:ro \
  --name lighttpd rocknsm/lighttpd
```
