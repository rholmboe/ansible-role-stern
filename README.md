# Ansible Role: Stern

[![CI](https://github.com/rholmboe/ansible-role-stern/workflows/CI/badge.svg?event=push)](https://github.com/rholmboe/ansible-role-stern/actions?query=workflow%3ACI)

Installs [Stern](https://github.com/stern/stern), a Go-based log tailer for kubernetes.

An honest duplication of [ansible-role-packer](https://github.com/geerlingguy/ansible-role-packer/) by [Jeff Geerling](https://www.jeffgeerling.com/)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
    stern_version: "1.20.1"
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
