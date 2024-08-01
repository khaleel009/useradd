###########################
Useradd 
###########################


sudo useradd -m <username> 
Ex: sudo useradd -m tom

sudo usermod -aG <groupname> <username> 
Ex: sudo usermod -aG git tom

sudo passwd -l <username>
 Ex: sudo passwd -l tom

To delete a password
su - git #This prompts for password to enter, if you want to disable.

sudo passwd -d git
sudo vi /etc/ssh/sshd_config # In this file "PermitEmptyPasswords yes" change it.
sudo systemctl restart ssh.service
