# The Language Bank AAI Server Creation

## Requirements
```
virtualenv -p python3 .venv
source .venv/bin/activate
pip install -r requirements_dev.txt
```
```
ansible-galaxy install -r requirements.yml
```

## Provisioning
Get and source [Pouta OpenStack RC file](https://docs.csc.fi/cloud/pouta/install-client/#configure-your-terminal-environment-for-openstack), then run
```
ansible-playbook -i inventories/development site.yml
```
