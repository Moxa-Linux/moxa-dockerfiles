Dockerfiles are provided for setup the environment to compile the kernel source of MOXA UC series products.

# Steps
## Prepare Dockcer environment

If having the docker installed, please skip this step.

Please refer to [official site](https://docs.docker.com/install/)

## Prepare docker image

Execute following command to build the docker image

```
$ cd stretch
$ sudo docker build -t moxa_docker:v1 ./
```

After the docker build, the images should be ready to use. Check with

```
$ docker images moxa_docker
```
