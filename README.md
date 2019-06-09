# odoosetup
setup instruction for odoo

## Install using docker
1. Login to docker
```
docker login
docker run -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo --name db postgres:10
docker run -t -p 8069:8069 --name odoo --link db:db odoo:12.0 -d odoo12
```
