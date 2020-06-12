# moxa-dockerfiles

moxa-dockerfiles provides the `dockerfile` for building develop environment to compile the kernel source, tools and libraries of Moxa Computer products.

## Steps

### Prepare docker environment

To prepare your docker environment, please visit page [Get Docker](https://docs.docker.com/get-docker/) for more information.

### Build your docker image

Before starting build docker image, please make sure you have already under the directory which `dockerfile` located.

Now we can start building docker image. For example, if we want build a docker image which named `moxa-package-builder` with tag `1.0.0`, execute following command:

```
$ sudo docker build -t moxa-package-builder:1.0.0 .
```

Once build process completed, you can check your docker image with following command:

```
$ sudo docker images moxa-package-builder
```
