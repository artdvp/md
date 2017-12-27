# Docker on kali

> Add Docker PGP key

```
$ curl -fsSL https://download.docker.com/linux/debian/gpg | sudo apt-key add -
```

> Configure Docker APT repository:

```
$ echo 'deb https://download.docker.com/linux/debian stretch stable' > /etc/apt/sources.list.d/docker.list
```

> Update APT

```
$ apt-get update
```

> Install Docker

```
$ apt-get remove docker docker-engine docker.io
$ apt-get install docker-ce

-- Test
$ docker run hello-world
```

> To start services:

```
$ systemctl start docker
$ systemctl enable docker
```
