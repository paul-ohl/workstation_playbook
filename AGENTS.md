# AGENTS.md

## Overview
This project is an Ansible playbook designed to automate the setup of a developer workstation. It uses roles to install and configure various tools and system settings, such as Docker, Rust, and system-level configurations.

## Build, Lint, and Test Commands

### Execution
- **Run the playbook**: `ansible-playbook -K playbook.yml`
  - The `-K` flag prompts for the `become` (sudo) password.
  - The inventory is configured in `ansible.cfg` to point to `hosts`.

### Linting
- **Run the linter**: `ansible-lint`
  - This command will lint all YAML files in the project based on the rules defined in `.ansible-lint`.

## Project Structure

- `playbook.yml`: The main entry point that defines the hosts and roles to be executed.
- `roles/`: Contains Ansible roles, which are self-contained units of automation for specific tasks (e.g., `rust_install`, `system`).
- `tasks/`: Holds ad-hoc tasks that can be imported into the main playbook.
- `group_vars/`: Contains variables for specific host groups.
- `ansible.cfg`: Configuration file for Ansible, specifying settings like inventory location.
- `requirements.yml`: Defines external role dependencies from sources like Ansible Galaxy.

## Code Style Guidelines

- **YAML**: Files use a 2-space indentation convention.
- **Naming**: Role and task names are descriptive and use snake_case (e.g., `rust_install`).

## Commit Style

Commit messages loosely follow the Conventional Commits format (e.g., `feat:`, `fix:`, `wip:`). It is recommended to adopt this style more formally for clarity.

- **Format**: `type(scope): summary`
- **Example**: `feat(docker): Add support for Docker Compose`
