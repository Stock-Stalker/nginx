<!-- logo -->
<p align="center">
  <img width="300" src="logo.png">
</p>

<!-- short description -->
<h1 align="center">StockStalker - Nginx Reverse Proxy </h1>

<p align="center">
    <!-- license -->
    <img src="https://img.shields.io/github/license/Stock-Stalker/nginx" />
    <!-- code size  -->
    <img src="https://img.shields.io/github/languages/code-size/Stock-Stalker/nginx" />
    <!-- issues -->
    <img src="https://img.shields.io/github/issues/Stock-Stalker/nginx" />
    <!-- pull requests -->
    <img src="https://img.shields.io/github/issues-pr/Stock-Stalker/nginx" />
    <!-- number of commits per year -->
    <img src="https://img.shields.io/github/commit-activity/y/Stock-Stalker/nginx" />
    <!-- last commit -->
    <img src="https://img.shields.io/github/last-commit/Stock-Stalker/nginx" />
    <!-- docker image size -->
    <img src="https://img.shields.io/docker/image-size/starlightromero/stockstalker-nginx" />
    <!-- docker pulls -->
    <img src="https://img.shields.io/docker/pulls/starlightromero/stockstalker-nginx" />
    <!-- website status -->
    <img src="https://img.shields.io/website?url=https%3A%2F%2Fstockstalker.tk" />
</p>


## Table of Contents

- [Make Commands](#make-commands)
- [Required Software](#required-software)
- [How to Run](#how-to-run)


## Make Commands

`stop`: Stop the running server

`rm`: Remove all unused containers

`rm-all`: Stop and remove all containers

`rmi`: Remove stockstalker images without removing base images. Useful for speeding up build time when switching from one start script to another such as `make start` to `make test`

`rmi-all`: Remove all images

`purge`: _Use with caution_ Completely purge Docker containers, networks, images, volumes, and cache

`build`: Build development server without running the server

`start`: Start development server at port `8080`

`reload`: Stop development server and restart the server at port `8080`

`hard-reload`: Stop container, remove container, rebuild container, and start development server

`debug`: Start development server in debug mode

`test-image-security`: Test security vulnerabilities for base images (must have [snyk](https://support.snyk.io/hc/en-us/articles/360003812538-Install-the-Snyk-CLI) installed globally)


## Required Software

- [Docker](https://docs.docker.com/get-docker/)
- [docker-comopse](https://docs.docker.com/compose/install/)
- [CMake](https://cmake.org/install/)


## How to Run

Clone the repo
```zsh
git clone git@github.com:Stock-Stalker/nginc.git
```

cd into the directory
```zsh
cd nginx
```

Run the application!
```zsh
make start
```

To stop the app press `CNTRL + C`. Then run:
```zsh
make stop
```