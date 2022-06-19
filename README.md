# des dockerfiles pour mes projects

## créer image

```bash
$ docker build -t monimage:tag . #(exemple tag : version)
```

## lister les images locales

```bash
$ docker ls
```

## lancer un container avec monimage

```bash
$ docker run -tid --name moncontainer monimage:tag
```

## lancer un terminal dans le container

docker exec -ti moncontainer /bin/bash