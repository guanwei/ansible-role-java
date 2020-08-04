# Ansible Role: Java

Installs Java on RedHat/CentOS or Debian/Ubuntu.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
```

## Dependencies

None.

## Example Playbook

requirements.yml
```
- name: java
  src: <repo_url>
  version: <branch_name>
  scm: git
```

playbook.yml
```
- hosts: servers
  roles:
    - java
```
