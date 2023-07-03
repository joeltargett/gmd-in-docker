# gmd-in-docker

This repository demonstrates, how we can run gmd in Docker.

## How to use

1. Create your own copy of `docker-compose.override.yml`:

   ```bash
   cp docker-compose.override.yml.sample docker-compose.override.yml
   ```

   Note, it's included in `.gitignore`.

1. Run:

   ```bash
   docker-compose up -d --build
   ```
   
1. Try accessing [http://localhost:8080/app](http://localhost:8080/app) in your browser.

1. Uninstall:

   ```bash
   docker-compose down
   ```

1. Remove persistent data:

   ```bash
   rm -rf data/configs
   rm -rf data/influxdb
   rm -rf data/logs
   ```
