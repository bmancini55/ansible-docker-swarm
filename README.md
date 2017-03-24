# ansible-docker-swarm
Ansible roles for bootstrapping a docker swarm cluster.

This consists of 3 different server types:
1. swarm leader (only one of these should exist)
2. swarm managers
3. swarm workers

This playbook will install Docker and initialize the swarm. Swarm commands are idempotent.

```
ansible-playbook -i test site.yml
ansible-playbook -i test --key-file=~/keys/test.pem --user ubuntu site.yml
```
