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

- Install kmonad (check [this](https://github.com/kmonad/kmonad/blob/master/doc/installation.md#using-docker) out)
