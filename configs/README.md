# IoD Configs

### Development

### [gpii-iod.dev](gpii-iod.dev.json5)

Server listens on port 8084, open to the world.

## Production

or, "production-*like*"

### [gpii-iod.production](gpii-iod.production.json5)

Server listens on port 18084, bound to localhost. External connectivity is provided by nginx.

## GCloud production configuration

This configuration was created to deploy gpii-iod in a docker container and inside a VM instance on Google Cloud.

* Server listens on port 8081 or port defined through the env variable `IOD_PORT`
* Packages folder needs to be provided through the `IOD_PACKAGES_FOLDER` env variable - if not provided, it defaults to `./testData/packages`
* No admin component/interface loaded into the coniguration
