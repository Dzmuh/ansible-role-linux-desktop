# Ansible setup Linux for Desktop

Ubuntu/Kubuntu 20.04 only

## Start

ansible-playbook ansible-linux-desktop.yml --ask-become-pass -vvv --check

## Using Tags


ansible-playbook ansible-linux-desktop.yml --ask-become-pass --tags "bootstrap,kde,firewall"
