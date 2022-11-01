# Possible Bug

Start Image

```bash
docker-compose up --build
```

Open the following http://localhost:8080/relay/app in your Browser to trigger the stick-table

Check Stick-Table inside Container

```bash
docker exec -ti haproxy_bug_haproxy_1 /bin/bash
echo "show table api" | socat stdio UNIX-CONNECT:/run/haproxy.sock
or
docker exec -ti haproxy_bug_haproxy_1 sh -c 'echo "show table api" | socat stdio UNIX-CONNECT:/run/haproxy.sock'
```
