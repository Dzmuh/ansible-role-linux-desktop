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
ansible-playbook ansible-linux-desktop.yml --ask-become-pass --tags "kde,firewall" -vvv --check
ansible-playbook ansible-linux-desktop.yml --ask-become-pass --tags "kde,firewall" --check
ansible-playbook ansible-linux-desktop.yml --ask-become-pass --tags "bootstrap,kvm" --check

## TODO

- [ ] stellarium
- [ ] mypaint
- [ ] mypaint-brushes
- [ ] default-jdk
