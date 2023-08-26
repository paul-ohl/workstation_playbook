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

- Fix issue with aptitude not reading dicts
- Cargo install checker is disgustingly made, fix it
- Put the rust toolchain install in a role
