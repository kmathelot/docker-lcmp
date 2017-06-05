# docker-lcmp
Caddy MySQL Php Stack Powered by docker

Idea :

Deploy web based applications, with docker services.

You need to install docker-ce and docker-compose

Configure your Caddyfile and put it into your project folder.  

```
Ex :

/your/path:
    - Caddyfile
    - index.php


Caddyfile sample :

localhost:80 {
  gzip
  fastcgi / php:9000 php
}
```

Change mounted volumes with your path.  

Certificates are in the .caddy path.  

Launch application with docker-compose up, see compose documentation for more information.

your application is accessible with your browser, curl or whatever can do http request.  
