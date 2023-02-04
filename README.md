# Ansible-update-packages

Ansible Playbook - Update all packages on servers

This Ansible playbook automates the task of updating all packages on multiple servers. It uses the apt module to upgrade all packages and update the package cache.

Requirements
Ansible 2.9 or later

A list of servers to run the playbook on, specified in the hosts file or an inventory file.

SSH access to the servers, with a user that has sufficient privileges to run the apt command.

Usage

Step 1: Clone or download this repository to your local machine.

Step 2: Edit the hosts file to specify the list of servers you want to run the playbook on.

Step 3: Run the playbook with the following command:

```ymal 
ansible-playbook update_packages.yml
```


Step 4: The playbook will update all packages on all servers specified in the hosts file.

Notes

The playbook assumes that the servers are running a Debian-based Linux distribution (e.g. Ubuntu). If the servers are running a different distribution, you may need to modify the playbook accordingly.

The playbook uses the become directive to run the tasks as a privileged user (e.g. root). Make sure the user specified in the ansible.cfg file has sufficient privileges to run the playbook.
