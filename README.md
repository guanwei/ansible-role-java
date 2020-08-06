# Ansible Role: Java

Installs Java on RedHat/CentOS or Debian/Ubuntu.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
# Java distribution type:
#  - openjdk
#  - adoptopenjdk
java_distribution: openjdk
java_major_version: 8
# supported jdk/jre
java_type: jdk

java_adoptopenjdk_apt_repository: "deb https://adoptopenjdk.jfrog.io/adoptopenjdk/deb/ {{ ansible_distribution_release }} main"

# AdoptOpenJDK Implementation (hotspot/openj9)
java_adoptopenjdk_impl: hotspot
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
