# dev_tools

Ansible scripts to setup dev environment.

## Usage

```bash
ansible-playbook --private-key {{ ansible deploy key }} -u {{ ansible user }} -i inventory.ini site.yaml -vvv

# node agent
ansible-playbook --private-key ~/.ssh/id_ed25519 -i inventory.ini node_agent.yml -vvv

# dev_tools
ansible-playbook --private-key ~/.ssh/id_ed25519 -u zhangjian -e user=zhangjian  -i inventory.ini dev_tools.yml -vvv

# gpu-operator
ansible-playbook --private-key ~/.ssh/id_ed25519 -i inventory.ini gpu-operator.yml -e "@extra-vars.yml" -vvv

# cuda
ansible-playbook --private-key ~/.ssh/id_ed25519 -i inventory.ini cuda.yml -e "@extra-vars.yml" -vvv
```

