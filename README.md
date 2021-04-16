# Ansible Role: Openrazer

[![CI](https://github.com/pmikus/ansible-role-openrazer/actions/workflows/CI.yml/badge.svg)](https://github.com/pmikus/ansible-role-openrazer/actions/workflows/CI.yml)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-openrazer&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-openrazer)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=pmikus_ansible-role-openrazer&metric=bugs)](https://sonarcloud.io/dashboard?id=pmikus_ansible-role-openrazer)

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    openrazer_package: "darktable"

Name of package in package repository.

    openrazer_package_state: "present"

Install package (optionally you can change to "absent" to uninstall).

    darktable_apt_state: "present"

Install APT repository (optionally you can change to "absent" to roll back).

    openrazer_apt_release_channel: "daily"

APT channel can be one of: "stable" or "daily".

## Dependencies

None

## Example Playbook

    - hosts: localhost
      roles:
        - pmikus.ansible-role-openrazer

## License

MIT / BSD

## Author Information

This role was created by [Peter Mikus](https://www.linkedin.com/in/petermikus/).
