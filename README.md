# Setup Docker for Odoo 10 with pgAdmin Access


### Install docker:
```
$ sudo apt install docker.io
$ sudo systemctl start docker
$ sudo systemctl enable docker
```

### Install docker compose:
```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo systemctl enable docker
```

### Start the container from the root of this project:
```
$ docker-compose up  -d
```

Then locate `localhost:10000` to access Odoo 10.0.

<img width="300px" src="https://raw.githubusercontent.com/odoo-10-docker/static/odoo-apps.png" alt="Odoo is working.">

Connect postgres now using pgAdmin using the following credentials.
```
name: admin@admin.com
host: localhost (if not matched, find hostname)
port: 5050
username: odoo
password: odoo
```

<img width="300px" src="https://raw.githubusercontent.com/odoo-10-docker/static/odoo-apps.png" alt="Odoo is working.">

