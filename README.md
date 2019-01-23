# docker-dockercompose install
docker & docker-compose installation

### A) Uninstall old version of docker
```bash
$ sudo apt-get remove docker docker-engine docker.io containerd runc
```

#### Remove all folders related to docker
```bash
$ sudo rm -rf /var/lib/docker
$ sudo rm -rf /etc/docker
$ sudo rm /etc/apparmor.d/docker
$ sudo groupdel docker
$ sudo rm -rf /var/run/docker.sock
$ sudo rm -rf /usr/local/bin/docker-compose

```

### B) Install fresh docker 

 1. Download installation script for docker in current directory 
   ```bash
   $ curl -fsSL https://get.docker.com -o get-docker.sh
   ```
 2.  

