# [bootstrap](#bootstrap)

Prepare your system to be managed by Ansible.

|GitHub|Version|Ansible Galaxy|Quality|Downloads|
|------|-------|--------------|-------|---------|
|[![github](https://github.com/ucomesdag/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg)](https://github.com/ucomesdag/ansible-role-bootstrap/actions)|[![version](https://img.shields.io/github/v/release/ucomesdag/ansible-role-bootstrap)](https://github.com/ucomesdag/ansible-role-bootstrap/releases/)|[![role](https://img.shields.io/ansible/role/00000)](https://galaxy.ansible.com/ucomesdag/bootstrap)|[![quality](https://img.shields.io/ansible/quality/00000)](https://galaxy.ansible.com/ucomesdag/bootstrap)|[![downloads](https://img.shields.io/ansible/role/d/00000)](https://galaxy.ansible.com/ucomesdag/bootstrap)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/resources/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: ucomesdag.bootstrap
```

## [Role Variables](#role-variables)

These variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for bootstrap


```

## [Dependencies](#dependencies)

Overview of role dependencies:

![dependencies](https://raw.githubusercontent.com/ucomesdag/ansible-role-bootstrap/png/requirements.png "Dependencies")

## [Requirements](#role-requirements)

- pip packages listed in [requirements.txt](https://github.com/ucomesdag/ansible-role-bootstrap/blob/master/requirements.txt).

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://quay.io/user/ucomesdag):

|container      |tags                     |
|---------------|-------------------------|
|alpine         |edge, latest             |
|amazonlinux    |latest                   |
|archlinux      |latest                   |
|centos         |latest, stream8          |
|debian         |latest, buster           |
|fedora         |rawhide, latest, 34, 33  |
|opensus        |latest                   |
|rhel           |latest                   |
|rocky          |latest                   |
|rpi-os         |latest                   |
|ubuntu         |jammy, latest, bionic    |

The minimum version of Ansible required is 2.10, tests have been done to:

- The previous version.
- The current version.
- The development version.

See the [Ansible community changelogs](https://docs.ansible.com/ansible/devel/reference_appendices/release_and_maintenance.html#ansible-community-changelogs) for details.

## [Exceptions](#exceptions)

Some variarations of the build matrix do not work. These are the variations and reasons why the build won't work:

| variation   | reason                                |
|-------------|---------------------------------------|
|             |                                       |


If you find issues, please register them in [GitHub](https://github.com/ucomesdag/ansible-role-bootstrap/issues)

## [License](#license)

Apache-2.0
