# [Ansible](https://www.ansible.com). Install Docker CE and Docker-Compose

This Playbook install [Docker CE](https://docs.docker.com/install/) and [Docker-Compose](https://docs.docker.com/compose/install/) on Ubuntu or CentOS server. OS version will be automatically determined.

## Requirements
* SSH root access to the target servers. 

How to do that: Copy your public key to the target server with command below:
```
ssh-copy-id root_user@target.server.com
```

## Usage
* In ./ansible.cfg - check path to your private key and username
* In ./group_vars/target - change the values you need
* In ./hosts - define Hostname or IP of target servers
* Run Playbook:
```
ansible-playbook docker-install.yml
```


