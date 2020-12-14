# Ansible - Install LAMP & Nginx-PHP 

Playbook to configure LAMP on Redhat Hosts & Nginx-PhP on Debian Hosts

Created 3 playbook files to perform this tasks

  - lamp-amazon.yaml 
  - nginx-ubuntu.yaml
  - nginx-httpd.yaml

# lamp-amazon.yaml
Install LAMP on Redhat Host
### 3 tasks
  -  Install LAMP service
  - Create index file
  - Restart services

## nginx-ubuntu.yaml
Install Nginx-PhP-Mysql on Debian Host

### 5 tasks
  - Upgrade all apt packages
  - Install Nginx , php & mysql service
  - Copy nginx default file"
  - Copy indxe.php  file contents
  - Restart services
 
## Other files
 - inventory.txt
 - default
 - nginx-httpd.yaml
 
## inventoty.txt

 - lists the hosts with ansible_user and ansible_ssh_private_key_file
 
## default

Once php installed we need to  pass PHP scripts to FastCGI server 

## nginx-httpd.yaml

Play book in which we include the above tasks 
