# Spring PetClinic

Spring Demo Application

## Description

## Demo
### Cloud Native Buildpacks
#### pack - Buildpack CLI

- MacOS 
```
$ brew install buildpacks/tap/pack
```

- Linux
```
$ wget https://github.com/buildpacks/pack/releases/download/v0.11.2/pack-v0.11.2-linux.tgz
$ tar xvf pack-v0.11.2-linux.tgz
$ rm pack-v0.11.2-linux.tgz
$ sudo mv pack /usr/local/bin/
```

#### Builder

- **Paketo Buildpacks**
- **Google Cloud Buildpacks**

`$ pack build --builder <BUILDER_NAME> <APP_NAME>`

#### Paketo Buildpack

Builder: **gcr.io/paketo-buildpacks/builder:base**

#### Google Cloud Buildpacks

Builder: **gcr.io/buildpacks/builder**

- `$ pack build --builder gcr.io/buildpacks/builder:v1 <APP_NAME>`
  - Google Container Registry: `--publish gcr.io/<YOUR_PROJECT_ID>/<APP_NAME>`
  - Docker Hub: `--publish docker.io/<YOUR_PROJECT_ID>/<APP_NAME>`

```
$ pack build --builder gcr.io/buildpacks/builder --publish docker.io/shinyay/spring-petclinic:1.0.0
```

#### Run Containr Application
```
$ docker run --rm -p 8080:8080 shinyay/spring-petclinic:1.0.0
```

#### Run on Cloud Run

[![Run on Google Cloud](https://deploy.cloud.run/button.svg)](https://deploy.cloud.run)

## Features

- feature:1
- feature:2

## Requirement

## Usage

## Installation

## Licence

Released under the [MIT license](https://gist.githubusercontent.com/shinyay/56e54ee4c0e22db8211e05e70a63247e/raw/34c6fdd50d54aa8e23560c296424aeb61599aa71/LICENSE)

## Author

[shinyay](https://github.com/shinyay)
