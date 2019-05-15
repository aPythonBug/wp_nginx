# WordPress + Nginx Ansible Playbook
Ansible playbook and roles for installing WordPress + Nginx + PHP + Postfix server

### Requirements
- Ansible 2.0.0 or newer
- Ubuntu 16.04 (installed on your web server or virtual machine)

### Instructions:

### 1. Configure your web server for ssh

Allow connections from your development machine to the web server over ssh. This is essential for ansible to work, so make sure to configure your remote or local server to allow connections via ssh. You may find `ssh-copy-id` helpful. 

### 2. Set the web server IP address

Change `192.168.100.10` from the file hosts to your server's URL or the IP address of your virtual machine:

```
[web-server]
192.168.100.10
```

### 3. Run the playbook

```
$ ansible-playbook playbook.yml -i hosts
```
