# des dockerfiles pour mes projects

## Ghpages

* image de base : debian bookworm slim
* paquets installés : github-pages

L'image créée contient le Gem de base pour obtenir un environnement comparable à ce que propose Github Pages :

* jekyll 	3.9.2
* github-pages-health-check 	1.17.9
* github-pages 	226
* html-pipeline 	2.14.1
* jekyll-avatar 	0.7.0
* jekyll-coffeescript 	1.1.1
* jekyll-commonmark-ghpages 	0.2.0
* jekyll-default-layout 	0.1.4
* jekyll-feed 	0.15.1
* jekyll-gist 	1.5.0
* jekyll-github-metadata 	2.13.0
* jekyll-include-cache 	0.2.1
* jekyll-mentions 	1.6.0
* jekyll-optional-front-matter 	0.3.2
* jekyll-paginate 	1.1.0
* jekyll-readme-index 	0.3.0
* jekyll-redirect-from 	0.16.0
* jekyll-relative-links 	0.6.1
* jekyll-remote-theme 	0.4.3
* jekyll-sass-converter 	1.5.2
* jekyll-seo-tag 	2.8.0
* jekyll-sitemap 	1.4.0
* jekyll-swiss 	1.0.0
* jekyll-theme-architect 	0.2.0
* jekyll-theme-cayman 	0.2.0
* jekyll-theme-dinky 	0.2.0
* jekyll-theme-hacker 	0.2.0
* jekyll-theme-leap-day 	0.2.0
* jekyll-theme-merlot 	0.2.0
* jekyll-theme-midnight 	0.2.0
* jekyll-theme-minimal 	0.2.0
* jekyll-theme-modernist 	0.2.0
* jekyll-theme-primer 	0.6.0
* jekyll-theme-slate 	0.2.0
* jekyll-theme-tactile 	0.2.0
* jekyll-theme-time-machine 	0.2.0
* jekyll-titles-from-headings 	0.5.3
* jemoji 	0.12.0
* kramdown-parser-gfm 	1.1.0
* kramdown 	2.3.2
* liquid 	4.0.3
* minima 	2.5.1
* nokogiri 	1.13.4
* rouge 	3.26.0
* ruby 	2.7.3
* safe_yaml 	1.0.5
* sass 	3.7.4

## Rappel : quelques commandes de bases docker 

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