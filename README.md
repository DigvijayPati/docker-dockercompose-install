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
   ubuntu@username:~$ curl -fsSL https://get.docker.com -o get-docker.sh
   ```
 2. Run script which will automatically install docker
   ```bash
   ubuntu@username:~$ sh get-docker.sh
   ```
 3. Add user to the docker group
   ```bash
   ubuntu@username:~$ sh get-docker.sh
   ```
 4. Reboot Machine

 5. Check the docker version
   ```bash
   ubuntu@username:~$ docker version 
    Client:
      Version:           18.09.1
      API version:       1.39
      Go version:        go1.10.6
      Git commit:        4c52b90
      Built:             Wed Jan  9 19:35:23 2019
      OS/Arch:           linux/amd64
      Experimental:      false

     Server: Docker Engine - Community
       Engine:
       Version:          18.09.1
       API version:      1.39 (minimum version 1.12)
       Go version:       go1.10.6
       Git commit:       4c52b90
       Built:            Wed Jan  9 19:02:44 2019
       OS/Arch:          linux/amd64
       Experimental:     false
   ```

 



