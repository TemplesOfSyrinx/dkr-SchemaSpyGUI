[GitHub]: https://github.com/TemplesOfSyrinx/dkr-SchemaSpyGUI
[GitHub_Tags]: https://github.com/TemplesOfSyrinx/dkr-SchemaSpyGUI/tags
[GitHub_Issues]: https://github.com/TemplesOfSyrinx/dkr-SchemaSpyGUI/issues
[GitHub_Forks]: https://github.com/TemplesOfSyrinx/dkr-SchemaSpyGUI/network
[DockerHub]: https://hub.docker.com/r/templesofsyrinx/dkr-schemaspygui
[DockerHub_Builds]: https://hub.docker.com/r/templesofsyrinx/dkr-schemaspygui/builds
# dkr-SchemaSpyGUI

| [GitHub] | [DockerHub] |
| -------- | ----------- |
| [![GitHub tags](https://img.shields.io/github/tag/TemplesOfSyrinx/dkr-SchemaSpyGUI.svg "GitHub tag")][GitHub_Tags]| [![Docker build](https://img.shields.io/docker/automated/templesofsyrinx/dkr-schemaspygui.svg "Docker build")][DockerHub_Builds]
| [![GitHub issues](https://img.shields.io/github/issues/TemplesOfSyrinx/dkr-SchemaSpyGUI.svg "GitHub issues")][GitHub_Issues]| [![Docker stars](https://img.shields.io/docker/stars/templesofsyrinx/dkr-schemaspygui.svg "Docker stars")][DockerHub]
| [![GitHub forks](https://img.shields.io/github/forks/TemplesOfSyrinx/dkr-SchemaSpyGUI.svg "GitHub forks")][GitHub_Forks]| [![Docker pulls](https://img.shields.io/docker/pulls/templesofsyrinx/dkr-schemaspygui.svg "Docker pulls")][DockerHub]

Docker container to run SchemaSpyGUI
 - Run SchemaSpyGUI in docker. 
 - Use x11docker to run image to be able to run GUI application from within docker image. 
 - Get [x11docker and x11docker-gui from github](https://github.com/mviereck/x11docker)

# Example command: 
 ```
 x11docker templesofsyrinx/dkr-schemaspygui:{VERSION}
 ```

# Without container isolation (less secure):
 ```
 xhost +local:docker
 docker run --rm \
    --env DISPLAY=unix$DISPLAY \
    --volume /tmp/.X11-unix:/tmp/.X11-unix \
    templesofsyrinx/dkr-schemaspygui:{VERSION}
 ```
