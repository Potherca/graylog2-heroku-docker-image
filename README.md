# Docker Image for running Graylog2 on Heroku

![graylog2-docker-heroku-logo](https://raw.githubusercontent.com/Potherca/graylog2-heroku-docker-image/master/graylog2-docker-heroku-logo.png)

This repository contains a Docker Image meant to run Graylog2 on Heroku

## Introduction

This is achieved by creating an Docker image based on [`heroku/cedar`](https://hub.docker.com/r/heroku/cedar/)[<sup>[1]</sup>](https://github.com/heroku/stack-images) which combines the content of the [`phusion/baseimage`](https://hub.docker.com/r/phusion/baseimage/)[<sup>[2]</sup>](https://github.com/phusion/baseimage-docker/tree/master/image) and [`graylog2/allinone`](https://hub.docker.com/r/graylog2/allinone/)[<sup>[3]</sup>](https://github.com/Graylog2/graylog2-images/tree/master/docker) images.

The result is [an image that is compatible with the Heroku Docker images](https://hub.docker.com/r/potherca/graylog2-heroku/) and can be run on Heroku using heroku-docker.

## Usage

To run the container locally execute the following command:

    docker run -t -p 9000:9000 -p 12201:12201 -p 12201:12201/udp potherca/graylog2-heroku

For more details please refer to [the Docker manual in the Graylog documentation](http://docs.graylog.org/en/latest/pages/installation/docker.html).

## Deployment

Details on deploying to Heroku are available in [the "Build and Deploy with Docker" reference in the Heroku devcenter](https://devcenter.heroku.com/articles/docker).

## License

The Source Code for this project is [available on github.com](https://github.com/Potherca/graylog2-heroku-docker-image) under [the GNU General Public License v3.0](LICENSE) (GPLv3) – Created by [Potherca](http://pother.ca/)
