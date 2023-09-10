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
- Install [Mononoki nerd font](https://objects.githubusercontent.com/github-production-release-asset-2e65be/27574418/6334d989-e832-4578-a511-54ef1848d66d?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20230905%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230905T084152Z&X-Amz-Expires=300&X-Amz-Signature=ee65174dc49ac82523038486e74aecc04d79496c0b193537bbe88f594e267e72&X-Amz-SignedHeaders=host&actor_id=37795294&key_id=0&repo_id=27574418&response-content-disposition=attachment%3B%20filename%3DMononoki.zip&response-content-type=application%2Foctet-stream)
    - It goes in `~/.local/share/fonts`
    - The ideal font size is 16
