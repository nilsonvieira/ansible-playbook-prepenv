# Introduction
## Requisites
### Install Needed Packs
```bash
sudo apt install ansible git openssh-server
```
### Configure Authorized_keys
The authorized_keys file needed been created on folder `/home/$USER/.ssh/` into user on server/computer.

This file can neeeded permissions 600
# How to use this Playbook
## Galaxy
Install the requirements with Ansible Galaxy.

```bash
ansible-galaxy install -r requirements.yml --roles-path roles
```
## Execute Playbook
```bash
ansible-playbook -i hosts site.yml -e usuario=$USER --ask-become-pass
```
# Distro Tests
- Pop!_OS 21.10