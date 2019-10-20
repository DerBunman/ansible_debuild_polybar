# ansible role debuild_polybar
Ansible cookbook to build and install a polybar .deb for Ubuntu/Debian.

# example
## playbook.yml
I install polybar on all hosts in the desktop group.
```yaml
- hosts: desktop
  roles:
    - derbunman.debuild_polybar
```

## requirements.yml
```yaml
- src: derbunman.debuild
- src: derbunman.debuild_polybar
```

## install dependencies
```sh
ansible-galaxy install -r requirements.yml
```

## update dependencies
```sh
ansible-galaxy install -r requirements.yml --force
```

## run playbook
```sh
ansible-playbook playbook.yml -v
```
