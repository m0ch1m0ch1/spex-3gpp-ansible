# Ansible Playbook for installing spex-3gpp on Ubuntu 20.04.3 LTS

[spex-3gpp](https://github.com/CoRfr/spex-3gpp) is a web service to deliver 3GPP specifications. This repository (spex-3gpp-ansible) is an Ansible Playbook for installing spex-3gpp on Ubuntu 20.04.3 LTS (including WSL2 environment). Running this playbook will install docker and deploy a container of spex-3gpp.

## Requirements

- Ansible 2.9.6 or newer
- Ubuntu 20.04.3 LTS

## Instructions

### 0. Update packages and install ansible

```
$ sudo apt update
$ sudo apt upgrade
$ sudo apt install ansible
```

### 1. Clone the repository and Run the playbook

```
$ git clone https://github.com/m0ch1m0ch1/spex-3gpp-ansible/
$ cd ./spex-3gpp-ansible
$ ansible-playbook playbook.yml -i hosts --ask-become-pass
```

### 2. Access spex-3gpp website

Open web browser and navigate to http://localhost:3000.