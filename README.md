# trojan-privoxy

trojan client with privoxy for http proxy

## How to use

```bash
docker run \
    --name trojan-proxy \
    -e REMOTE_ADDR="trojan server host" \
    -e REMOTE_PORT=<trojan server port> \
    -e PASSWORD="your password" \
    -p <socks5_trojan_port>:1086 \
    -p <http_privoxy_port>:1087 \
    -d \
    webee/trojan-privoxy
```
