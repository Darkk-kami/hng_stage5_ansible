# hng_stage5_ansible
## Automated Deployment and Configuration for NestJS application
This project automates the deployment and configuration of a NestJS application along with RabbitMQ setup on a remote server. It also configures the firewall to allow specific ports. The setup uses Ansible to ensure all tasks are performed reliably and consistently.

## Prerequisites
* Ansible installed on your local machine
* Ubuntu or a compatible Linux distribution
* Access to a remote server with sudo privileges
 
## Deployment
Create an inventory file named inventory.cfg with the following structure:
```
[webserver]
your_server_ip

[all:vars]
ansible_ssh_user=your_ssh_user
ansible_ssh_private_key_file=/path/to/your/private_key

```
Start the ansible script
```
ansible-playbook main.yaml -b
```

