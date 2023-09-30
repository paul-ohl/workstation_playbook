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

- Make some packages mandatory, others optional in the variables
- Change the kmonad service file to a template to be able to modify the username
- Finish adding the other services to tendresse
- Add 2FA automatic setup (test on a VM)
- Fix the ssh juggle fail (gl)
- Update the workstation config to use some of the server's roles
- Fix the nvim install task
- Setup a LDAP
- Configure Vaultwarden to use the LDAP
- Setup ansible secrets
- Look into MSMTP mailing and such
