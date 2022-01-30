# Introduction to Docker

Docker is an engine that automates the deployment of software packages (and its dependencies). It relies on a feature called OS-level virtualization, whereby the OS kernel allows for the existence of multiple isolated user space instances called *containers*.

## 1. Containers

```sh
docker create -it --name example ubuntu
docker start -i example
```

Now, we are inside a container called example. Note that there we cannot ping www.google.com from within our container, the reason being that iputils-ping is not installed by default in the Ubuntu *image* (We will learn more about docker images soon!). We can install the package, first run

```sh
apt update
apt upgrade -y
```
Then, run

```sh
apt install iputils-ping
```

Let us try that again running

```sh
ping www.google.com
```

```sh
docker ps
```

## 2. Network

## 3. Volumes

## 4. Images

## 5. Dockerfile

## 6. Docker compose
