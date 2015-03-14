# Ansible deployment scripts

Ansible deployment scripts and spikes for a bigger setup

### Directory structure

Uses [best practices](http://docs.ansible.com/playbooks_best_practices.html) structure.
The folder `inv` has a collection of inventories. One file per environment.

### Running spikes

Run spikes altogether
```
ansible-playbook -i inv/devbox spikes.yml 
```
or by tag. For example
```
ansible-playbook -i inv/devbox spikes.yml --tags=release
```

