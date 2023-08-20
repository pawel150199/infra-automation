# Ansible Automation

## This repository present developed by myself roles and playbooks to automate infrastracture provisioning to my projects

I have servers in hetzner cloud and developed those roles/playbooks to automate some configuration step.

## Requirements

This playbook should works on redhat family server, version 9 withour any dependencies.

### Keys
To run playbooks ssh private key is needed so keys should be placed in keys directory

## Example Playbook

"""yaml
- hosts: all
  become: true
  roles:
    - docker
"""
