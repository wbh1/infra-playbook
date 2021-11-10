# Ansible Infra Playbook
This repo houses my site playbook for my personal infrastructure.

## Requirements
1. Ansible >=2.9
2. Install the required roles to the `./roles/` directory
   1. `ansible-galaxy role install -r roles/requirements.yml`
3. Install required collections 
   1. `ansible-galaxy collection install -r roles/requirements.yml`
4. Ansible Vault password located at `~/.vault_pass`

## Usage
`ansible-playbook site.yml`

### Bootstrapping
`ansible-playbook -l newhost.hegedus.wtf site.yml --tags bootstrap`