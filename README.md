# Node-Red with Traefik

This Node-Red instance is secured with [Authelia](https://www.authelia.com/) by default.

To remove Authelia, which is not recommended, remove the following label:

```yaml
traefik.http.routers.${PROJECT_IDENTIFIER}.middlewares: 'chain-authelia@file'
```

## Configuration

To change the domain, change the variable `VIRTUAL_HOST` in the .env file.

To change the identifier for Traefik change the variable `PROJECT_IDENTIFIER` in the .env file.

To change the timezone change the variable `TIMEZONE` in the .env file.

---

Install Traefik: [Traefik with Authelia](https://github.com/erkenes/docker-traefik)