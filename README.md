# StockStalker - Backend API

## Makefile Commands

`stop`: Stop the running server

`rm`: Remove all unused containers

`rm-all`: Stop and remove all containers

`rmi`: Remove stockstalker images without removing base images. Useful for speeding up build time when switching from one start script to another such as `make start` to `make test`

`rmi-all`: Remove all images

`purge`: _Use with caution_ Completely purge Docker containers, networks, images, volumes, and cache

`build`: Build development server without running the server

`start`: Start development server at port `8080`

`reload`: Stop development server and restart the server at port `8080`

`debug`: Start development server in debug mode

`start-prod`: Start the production server

`debug-prod`: Start the production server in debug mode

## How to Run

To run the app you will need:

- [Docker](https://docs.docker.com/get-docker/)
- [docker-compse](https://docs.docker.com/compose/install/)

Once you have your environment fully set up, run:

```bash
make start
```

To stop the app press `CNTRL + C`. Then run:

```bash
make stop
```
