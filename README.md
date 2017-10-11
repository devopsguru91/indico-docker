# indico-docker

Simple Docker config to try Indico out.

```sh
$ docker-compose up
```

To run Indico with your own external database (prevents running postgres container), make sure you properly configure
the environment variables for `indico-web` service in `docker-compose.yml` (`PGHOST`, `PGUSER`, `PGPASSWORD`,
`PGDATABASE` and `PGPORT`) and run the following command instead:

```sh
$ docker-compose up indico-web indico-nginx
```

Access your instance through [localhost:8080](http://localhost:8080)
