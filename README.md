# PyCon APAC 2015 Site

## Sample Usage

```
> cd 2015apac # optional
> python3 -m http.server
```

### Run in docker

By default, this docker application listen on 8045 port.

Modify docker-compose file id needed.

```
> docker compose up # Add --build flag if needed
```

When used in production environment, you may add following
setting into nginx configuration.

```
	location /2015apac/ {
		proxy_pass http://127.0.0.1:8015/;
	}
```
