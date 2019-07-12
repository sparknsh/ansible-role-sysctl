# Ansible Role: sysctl

#### Version: 1.0.1

[![](https://img.shields.io/badge/role-sparknsh.sysctl-blue.svg)](https://galaxy.ansible.com/sparknsh/sysctl)

Development of this project is managed in a private repository then pushed out to [GitLab](https://gitlab.com/sparknsh/ansible-role-sysctl) and [GitHub](https://github.com/sparknsh/ansible-role-sysctl) when we have a new version for you. If you have any issues please contact [sparknsh](https://www.sparknsh.com/contact?type=issue&name=ansible-role-sysctl)

## Role Variables

```yaml
sysctl__file_name: ansible
sysctl__conf: []
```

#### Example

```yaml
sysctl__conf:
  - name: net.ipv4.tcp_fin_timeout
    value: 10
  - name: vm.swappiness
    value: 10
    state: absent
```

## Example Playbook

```yaml
- hosts: all
  vars_files:
    - vars/main.yml
  roles:
     - { role: sparknsh.sysctl }
```

## License

MIT

## Author Information

This role was created in 2019 by [sparknsh](https://www.sparknsh.com) at [Rebel Media, Inc.](https://www.rebelmedia.io/)
