# docker-teamspeak-app

## RUN

```
mkdir -p /teamspeak/mariadb/data
```

```
docker app run watchdg/teamspeak-app --name teamspeak
```

### default parameters.yml

```yml
teamspeak:
  mariadb:
    password: vermin-zombie-arbiter-regiment-boundary-come-glottal-tenon
    database: teamspeak
    volume: /teamspeak/mariadb/data
```

### or with custom parameters.yml

```
docker app run watchdg/teamspeak-app --name teamspeak --parameters-file my-parameters.yml
```

## BUILD

```
docker app build . -t my-teamspeak-app
```
