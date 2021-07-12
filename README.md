# 26thmay_B1_DEVOPS

Q1 
## Install Docker

### Update the apt package index and install packages to allow apt to use a repository over HTTPS:
```
$ sudo apt update
$ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

### Add Docker’s official GPG key: 
```
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

### Use the following command to set up the stable repository. To add the nightly or test repository, add the word nightly or test (or both) after the word stable in the commands below.
```
$ echo \
    "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

## Install Docker Engine

### Update the apt package index, and install the latest version of Docker Engine and containerd, or go to the next step to install a specific version:
```
$ sudo apt-get update
$ sudo apt-get install docker-ce docker-ce-cli containerd.io
```

###
```
$ sudo groupadd docker
```

```
$ sudo usermod -aG docker $USER
```

```
$ newgrp docker
```
### To check status of Docker
```
$ sudo systemctl status docker
``` 
<img src=statusdocker.png>

Q2
## Pull ubuntu:20.04 docker image

```
$ docker pull ubuntu:20.04
```
<img src=pullimage.png>

Q3
## Perform start ,stop and pause operations on a container made from ubuntu:20.04 image.










