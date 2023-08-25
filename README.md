# Ansible Role: Stern

[![CI](https://github.com/rholmboe/ansible-role-stern/actions/workflows/ci.yml/badge.svg)](https://github.com/rholmboe/ansible-role-stern/actions/workflows/ci.yml)
[![Ansible Role](https://img.shields.io/ansible/role/57220?logo=ansible)](https://galaxy.ansible.com/rholmboe/stern)
[![Ansible Quality Score](https://img.shields.io/ansible/quality/57220?logo=ansible)](https://galaxy.ansible.com/rholmboe/stern)

Installs [Stern](https://github.com/stern/stern), a Go-based log tailer for kubernetes.

An honest duplication of [ansible-role-packer](https://github.com/geerlingguy/ansible-role-packer/) by [Jeff Geerling](https://www.jeffgeerling.com/)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
    stern_version: "1.26.0"
```

The Stern version to install.

```
    stern_arch: "amd64"
```

The system architecture (e.g. `386` or `amd64`) to use.

```
    stern_bin_path: /usr/local/bin
```

The location where the Stern binary will be installed (should be in system `$PATH`).

The user/group which should own binary.

```
    stern_user: "root"
    stern_group: "root"
```

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - rholmboe.stern

## License

MIT / BSD

## Author Information

This role was created in 2021 by [Richard Holmboe](https://about.me/rholmboe)
