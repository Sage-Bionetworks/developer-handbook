Title: Containerizing Applications
Lang: en
Category: development
Slug: containerizing-applications
Summary: 
Status: draft

* this page needs much more work*

* the [ci-examples](https://github.com/Sage-Bionetworks-IT/ci-examples) repository contains github actions workflows for building docker images and pushing to docker hub and ghcr
* Some useful Docker base images include:
    * Python
    * Alpine/Ubuntu/Slim images
    * [R: best practices with docker](https://www.r-bloggers.com/2021/05/best-practices-for-r-with-docker/)

| Base Docker Image | Use Cases |
| -|-|
| [ubuntu](https://hub.docker.com/_/ubuntu) | larger images, but you might want to use this if you're creating a development environment |
| [alpine](https://hub.docker.com/_/alpine) | building a tool for publishing / desiring very smallest possible footprint |
| [python:3.x](https://hub.docker.com/_/python) | |
| [python:3.x-slim](https://hub.docker.com/_/python?tab=tags&page=1&name=slim) | |
| [rhub/r-minimal](https://github.com/r-hub/r-minimal) | Alpine linux-based R instance, small image size |
| [rocker/r-base](https://hub.docker.com/r/rocker/r-base/) | R instance, usually bleeding edge when it comes to system dependencies |
| [rocker/r-ubuntu](https://hub.docker.com/r/rocker/r-ubuntu) | Long-term support for ubuntu |
| [rocker/r-base](https://hub.docker.com/r/rstudio/r-base) | Long-term support for ubuntu |