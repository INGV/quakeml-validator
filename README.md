[![License](https://img.shields.io/github/license/INGV/quakeml-validator.svg)](https://github.com/INGV/quakeml-validator/blob/master/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/INGV/quakeml-validator.svg)](https://github.com/INGV/quakeml-validator/issues)

![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/ingv/qml-validator)
![Docker Image Size (latest semver)](https://img.shields.io/docker/image-size/ingv/qml-validator?sort=semver)
![Docker Pulls](https://img.shields.io/docker/pulls/ingv/qml-validator)

# quakeml-validator [![Version](https://img.shields.io/badge/dynamic/yaml?label=ver&query=softwareVersion&url=https://raw.githubusercontent.com/INGV/quakeml-validator/master/publiccode.yml)](https://github.com/INGV/quakeml-validator/blob/master/publiccode.yml)

This tool validate an XML file with QuakeML-1.2.xsd schema

## Quickstart
### Docker image
To obtain *qml-validator* docker image, you have two options:

#### 1) Get built image from DockerHub (*preferred*)
Get the last built image from DockerHub repository:
```
$ docker pull ingv/qml-validator
```

#### 2) Build by yourself
First, clone the git repository
```
$ git clone https://github.com/INGV/qml-validator.git
$ cd qml-validator
$ docker build --tag ingv/qml-validator .
```

in case of errors, try:
```
$ docker build --no-cache --pull --tag ingv/qml-validator .
```

### Run docker
```
$ docker run -it --rm -v $(pwd)/your_file_to_validate.xml:/opt/input.xml ingv/qml-validator
```

### Example screenshot
![alt text](images/screen.png)

# Contribute
Please, feel free to contribute.

# Author
(c) 2019 Valentino Lauciani valentino.lauciani[at]ingv.it

Istituto Nazionale di Geofisica e Vulcanologia, Italia
