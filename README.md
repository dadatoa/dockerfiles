# des dockerfiles pour mes projects

## Ghpages

* image de base : debian bookworm slim
* paquets installés : github-pages

L'image créée contient le Gem de base pour obtenir un environnement comparable à ce que propose Github Pages :
* Jekyll 3.9
* minima 2.5


### créer image

```bash
$ docker build -t monimage:tag . #(exemple tag : version)
```

### lister les images locales

```bash
$ docker ls
```

### lancer un container avec monimage

```bash
$ docker run -tid --name moncontainer monimage:tag
```

### lancer un terminal dans le container

docker exec -ti moncontainer /bin/bash