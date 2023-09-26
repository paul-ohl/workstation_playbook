# Fedora workstation ansible playbook

This is my ansible playbook to setup my fedora workstation(s).

## Usage

1. Read and edit variables in `groups_vars/all/vars.yml`.

2. To install dependencies:
```bash
ansible-galaxy install -r requirements.yml
```

3. To run: 
```bash
ansible-playbook -K playbook.yml
```

## TODO

- Use handler files when applicable
    - source: https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html#task-and-handler-organization-for-a-role
- Make some packages mandatory, others optional in the variables
- Add a "User setup" role with user, ssh and sudo configuration. copy ssh stuff from servers
- Change the kmonad service file to a template to be able to modify the username
