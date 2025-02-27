# Generic IOC Template Repository ioc-terminalserver

## Description
A Generic IOC for the terminal server

## Template Info
This repository was generated by
[ioc-template](https://github.com/epics-containers/ioc-template)

To update to the latest version of the template:

```bash
# activate a python virtual environment

pip install copier
cd ioc-terminalserver
copier update -a --trust .
```

## Developer Container

This repository includes a developer container configuration for Visual Studio Code. This allows you to run the Generic IOC locally and debug it. See https://epics-containers.github.io/main/tutorials/dev_container.html.

### IMPORTANT: First Time Preparation

The devcontainer uses a docker network that it can share with a ca-gateway in order that your PVs are accessible from your host machine. We arrange to create this network once and as long as you don't delete it or reset docker it will be available for all your devcontainers going forward.

To create the network run the following commands:

```bash
cd ioc-adsimdetector
source ./compose/environment.sh
```

