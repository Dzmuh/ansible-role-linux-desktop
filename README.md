# Ansible setup Linux for Desktop

Ubuntu/Kubuntu 20.04 only

## Start

Debug:

``` bash
ansible-playbook ansible-linux-desktop.yml --ask-become-pass -vvv --check
```

Run

``` bash
ansible-playbook ansible-linux-desktop.yml --ask-become-pass
```

## Using Tags


ansible-playbook ansible-linux-desktop.yml --ask-become-pass --tags "bootstrap,kde,firewall"
