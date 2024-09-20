# Advanced Linux

## Домашнє завдання

### 1) Install nginx:
#### sudo apt install -y nginx
![Pic2](02_nginx_ubuntu.png)

### 2) Add repository
#### sudo apt-add-repository ppa:ansible/ansible
![Pic3](03-add_rep.png)

### 3) delete repository
#### sudo apt-add-repository --remove ppa:ansible/ansible
![Pic4](04-del_rep.png)

#### sudo apt -y install ppa-purge
![Pic5](05-ppa-purge.png)


### File for service myserv
![Pic6](06-service.png)

### File for timer myserv
![Pic8](08-timer.png)

### Log for service myserv
![Pic10](10-var-log.png)


## Firewall configuration
### Allow SSH
#### sudo ufw allow ssh

### Disable All from 192.168.0.111
#### sudo ufw deny from 192.168.0.111

### Firewall status
![Pic11](11-ufw_status.png)
