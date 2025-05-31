# Git Setup Role

## Description

Ansible role to setup Git with comprehensive configuration.

## Variables

- `git_user_name`: Git global user name
- `git_user_email`: Git global user email
- `git_config_global`: Enable global Git configuration (default: true)
- `git_install_extras`: Install additional Git packages (default: true)
- `git_extra_packages`: List of extra Git-related packages to install

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: git-setup
      vars:
        git_user_name: "Deployment Team"
        git_user_email: "deploy@company.com"
```
