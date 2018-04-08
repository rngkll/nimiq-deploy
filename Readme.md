# Nimiq ansible deply recipe

This ansible playbook repository is intended to install a nimiq miming node.

The playbooks were tested using debian stable

Ansible will connect to the hosts specified in the inventory and run all the commands needed to have a nimiq miner.

## Get ansible
Installation instructions can be found [https://docs.ansible.com/ansible/intro_installation.html](here)

## Running the playbooks

### Modify variables
Important varaibles are located in one file `group_vars/all`

### Files needed
Copy inventory.example to inventory file and modify as needed.

### Run the playbook
modify the inventory file as needed
run 
`ansible-playbook -i inventory site.yml --ask-pass --ask-become-pass`

To limit ansbible to one specific server use the option `--limit <servername>`
