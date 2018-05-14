# eirka-provision
Packer/Ansible provisioning for eirka on Ubuntu 18.04

##### Build image:

    packer build -var 'digitalocean_key=' eirka.json

##### Provision eirka on instance created from image:

    ansible-playbook post.yml -i 10.0.0.1, -e 'ansible_python_interpreter=/usr/bin/python3'  
