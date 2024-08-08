
# Ruby 2.7.8 Docker Image

This repository contains a Dockerfile for building a Docker image of Ruby 2.7.8 based on Debian Bookworm. The image includes the OpenSSL extension patched to version 3.2.0 and upgrades to any Ruby gems with known security issues.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Building the Image](#building-the-image)
- [Running the Container](#running-the-container)
- [Included Components](#included-components)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

- Docker installed on your machine. You can download it from [here](https://www.docker.com/products/docker-desktop).

## Building the Image

To build the Docker image, clone this repository and run the following command in the directory containing the Dockerfile:

```sh
docker build -t ruby:2.7.8-bookworm .
```

This command will create a Docker image tagged as `ruby:2.7.8-bookworm`.

## Running the Container

To run a container using the created image, use the following command:

```sh
docker run -it --rm ruby:2.7.8-bookworm
```

This will start an interactive Ruby session.

## Included Components

- **Ruby 2.7.8**: The main programming language installed in the image.
- **Debian Bookworm**: The base OS for the image.
- **OpenSSL 3.2.0**: The OpenSSL extension patched to the version 3.2.0.
- **Security Updates**: Ruby gems with known security issues have been upgraded to their latest versions.

### Dockerfile Overview

The Dockerfile in this repository is based on the official [Docker Library Ruby](https://github.com/docker-library/ruby/blob/master/3.1/bookworm/Dockerfile) image for Debian Bookworm. The following customizations have been made:

- Ruby 2.7.8 installation.
- OpenSSL extension patched to version 3.2.0.
- Upgrades to Ruby gems with known security issues.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with your changes.

## License

This project is licensed under the MIT License.
