#### Publishing setup

```


docker buildx create --use
```

### AMD 64
```
docker buildx build -t saikpr/caddy-cloudflare:latest --push  .
docker buildx build -t saikpr/caddy-cloudflare:amd64 --push  .
```

### ARM 64
```
docker buildx build --platform linux/arm/v7,linux/arm64/v8,linux/amd64 -t saikpr/caddy-cloudflare:latest --push  .
docker buildx build -t saikpr/caddy-cloudflare:arm64 --push  .

```
