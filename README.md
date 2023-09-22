# Fedora workstation ansible playbook

This is my ansible playbook to setup my fedora workstation(s).

To install dependencies:
```bash
ansible-galaxy install -r requirements.yml
```

To run: 
```bash
ansible-playbook -K playbook.yml
```

## TODO

- refactor OS-specific actions
    - source: https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html#operating-system-and-distribution-variance
- Use handler files when applicable
    - source: https://docs.ansible.com/ansible/2.8/user_guide/playbooks_best_practices.html#task-and-handler-organization-for-a-role
- Make some packages mandatory, others optional in the variables
