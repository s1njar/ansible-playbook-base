# Homepage - Ansible
The ansible configuration for setting up and configuring db and redis.

# Usage

## Preparation
1. Install ansible on executor machine. [Link](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) 
2. Add ssh key to destination machine. 

## Run
```bash
# Run production
ansible-playbook playbook.yml -i env/prod/inventory.yml
```

## Add new role

```bash
# Execute
git submodule add <git_url> roles/<vendor.service>

# Example
git submodule add https://github.com/geerlingguy/ansible-role-mysql.git roles/geerlingguy.mysql
```

