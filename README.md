# docker-postgresql
My postgresql images

## Usage
Start postgresql in background
```
$ docker-compose up -d
```

Print bound port
```
$ docker port docker-postgresql 5432 | cut -d: -f2
```

And connect to postgresql
```
$ psql -h localhost -p `docker port docker-postgresql 5432 | cut -d: -f2` -U postgres
```
