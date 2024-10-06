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

### Deny ssh from IP
![Pic12](12-ufw_ssh_deny.png)

## Fail2ban configuration

### sudo apt install fail2ban -y
### sudo systemctl enable fail2ban
![Pic15](15-fail2ban_sys.png)

### sudo systemctl restart fail2ban.service
![Pic16](16-fail2ban_conf_log.png)


## Add new disk and automount

### Partition View 
![Pic21](21-NoDisk.png)

### Create disk
![Pic22](22-CreateDisk.png)
![Pic23](23-CreateDisk2Gb.png)
![Pic24](24-CreateDisk2GbFinish.png)

### Run fdisk
![Pic25](25-Disk2Gb_sdc.png)
![Pic26](26-Disk2Gb_sdc1.png)

### Format new disk
![Pic27](27-Disk2Gb_sdc1_id.png)

### Make Dir and mount drive
![Pic28](28-Disk2Gb_mount.png)

### Add mount (/etc/fstab)
![Pic29](29-Disk2Gb_fstab.png)

### Restart and verify automount
![Pic30](30-Disk2Gb_restart.png)


