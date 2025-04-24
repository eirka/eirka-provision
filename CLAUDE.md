# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build/Deployment Commands
- Build image: `packer build -var 'digitalocean_key=' eirka.json`
- Run provisioning: `ansible-playbook post.yml -i <host>, -e 'ansible_python_interpreter=/usr/bin/python3'`
- Upgrade Go: `ansible-playbook upgrade_go.yml -i <host>, -e 'ansible_python_interpreter=/usr/bin/python3'`

## Code Style Guidelines
- YAML files use 2-space indentation
- Use descriptive names for Ansible tasks
- Follow existing formatting patterns in configuration files
- Maintain consistent commenting style in config files
- Use kebab-case for service names
- Handle errors consistently across playbooks
- Keep tasks focused and atomic
- Group related tasks logically
- Use variables for reusable values
- Follow existing conventions when modifying configuration templates

This is primarily an infrastructure provisioning repo for the eirka web application using Ansible and Packer on Ubuntu.