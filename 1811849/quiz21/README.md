# How to create an Ansible Configuration  
1. Before creating an ansible configuration, check if ansible was installed on your machine using the command `ansible --version` . If not installed, use the command `apk add ansible` .  
1. Create the configuration file using the command `touch ansible.cfg` .  
1. To open and edit the configuration file, use the command `vim ansible.cfg` .  
1. Inside the configuration file add the information of your remote machine, add the inventory, remote user and privilege escalation.  
1. Save the configuration file.  
  
# How to create an Ansible Inventory  
1. Create the ansible inventory using `vim` or `touch` . Example: `vim inventory` .  
1. You will store the IP address of your remote machine on the inventory file.  
1. Users can also group their remote machine inside the inventory file. Example: `[group1]` .  
1. Save the inventory file.  

# How to create an Ad-hoc Ansible command with _setup_ and _shell_ module  
1. Use `ls` to view the configuration and inventory file.
1. To learn more Ad-hoc commands use this link: <https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html>  
1. Try to ping the remote user using the command `ansible all -m ping` . If the configuration and inventory are done properly the output should return with a `pong`.  
1. To input linux commands use the shell module, example: `ansible all -m shell -a "whoami"`.  
  
### Louis Adrian Mendoza  
