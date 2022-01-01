# Docker & Containerisation
Running docker container for a simple website.

## Table of contents
* [About](#about)
* [Demo](#demo)
* [Installation](#installation)

## About
In this repo, we are going to build a docker image that can run a simple website using official build of image [Nginx](https://hub.docker.com/_/nginx).


## Demo 
Check out the demo:
<p align="center"><img src="https://github.com/nekoemperor/website-docker/blob/master/images/web-docker.gif" width="768"  />

## Installation
* See the docker documentation for installation [docker](https://docs.docker.com/get-docker/)
* Clone this repo
* In the terminal, go to the root folder of this repo
* run ```docker build -t web-docker:latest .``` 
* then, ```docker run --name web-docker -p 9080:80 -d web-docker:latest ``` 
