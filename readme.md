# Node Stencil Docker Image

BigCommerce Stencil image.

Based on:
- Ubuntu 18.04
- npm 6.14.16
- Node v12.22.10

Created and tested on:
- Linux Mint 20.2
- Docker 20.10.12
- Docker Compose 1.29.2

## Build 

`docker build -t node_stencil .`

## Run

`docker run -it -v <theme_local_path>:/theme -p3000:3000 node_stencil bash`

Example: `docker run -it --name my_node_stencil -v $(pwd)/themes/cornerstone:/theme -p3000:3000 node_stencil bash`

## Stencil commands

Just run `npm` and `stencil` commands inside the container as usual.

- Npm install: `npm i`
- Stencil init: `stencil init`
- Stencil start: `stencil start`
- Stencil start with variation: `stencil start -v Bold`
