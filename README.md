# Fedora workstation ansible playbook

This is my ansible playbook to setup my fedora workstation(s).

To install dependencies:
```bash
ansible-galaxy install -r requirements.yml
```

To run: 
```bash
ansible-playbook -K run.yml
```

## TODO

- Install kmonad, resources:
    - https://github.com/kmonad/kmonad/blob/master/doc/installation.md#using-docker
    - https://docs.ansible.com/ansible/latest/collections/community/docker/docker_image_module.html
    - https://docs.ansible.com/ansible/latest/collections/community/docker/docker_container_module.html
