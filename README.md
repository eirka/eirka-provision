# eirka-provision
packer/ansible provisioning for eirka on ubuntu 16.04

##### Build image:

    packer build eirka.json

##### Provision eirka on instance created from image:

    ansible-playbook post.yml -i 10.0.0.1,
