# webMethods Template for Service Development # 01 - Quick Start and Fundamentals

## Quick Start

- Clone this repo
- Go to folder `02-run-configs/wmt-sd01-dev1`
- copy `EXAMPLE.env` into file `.env`
  - provide necessary licenses if running versions older than 11
  - ensure you can pull the images mentioned in the `.env` file
- Issue the command `docker compose up -d`
- Open Designer and point it to `http://localhost:40155` or better `http://host.docker.internal:40155`
- Develop your services and observe the changes to be staged and committed using a git client

## Creating Packages

- Copy the EmptyPackage folder in a folder named after your package name
  - Note that only `manifest.v3` is required in the folder so that Integration server recognizes it as a package. Everything else will accumulate in the folder during the service development phase using designer
- Mount the new folder in the `packages` folder in the `docker-compose.yml` file. Follow the given example
