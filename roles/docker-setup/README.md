# Docker and Docker Compose Setup Role

## Description

Ansible role to install and configure Docker and Docker Compose.

## Variables

- `docker_install`: Boolean to control Docker installation (default: true)
- `docker_edition`: Docker edition to install (default: 'ce')
- `docker_package_state`: Package installation state (default: present)
- `docker_users`: List of users to add to docker group
- `docker_compose_version`: Docker Compose version (default: 'v2')

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: docker-setup
      vars:
        docker_install: true
        docker_users:
          - deployer
          - alfiang
```
