# [bootstrap](#bootstrap)

Prepare your system to be managed by Ansible. This role will install the basic requirements (e.g., Python, sudo, etc.) necessary for the system to be managed by Ansible.

| GitHub                               | Version                                 | License                                 | Ansible Galaxy                   | Downloads                               |
|--------------------------------------|-----------------------------------------|-----------------------------------------|----------------------------------|-----------------------------------------|
|[![github][github-badge]][github-link]|[![version][version-badge]][version-link]|[![license][license-badge]][license-link]|[![role][galaxy-badge]][galaxy-link]|[![downloads][download-badge]][download-link]|

[github-link]: https://github.com/ucomesdag/ansible-role-bootstrap/actions
[version-link]: https://github.com/ucomesdag/ansible-role-bootstrap/releases
[license-link]: https://github.com/ucomesdag/ansible-role-bootstrap/LICENSE
[galaxy-link]: https://galaxy.ansible.com/ui/standalone/roles/ucomesdag/bootstrap/
[download-link]: https://galaxy.ansible.com/ui/standalone/roles/ucomesdag/bootstrap/versions/

[github-badge]: https://github.com/ucomesdag/ansible-role-bootstrap/workflows/Ansible%20Molecule/badge.svg
[version-badge]: https://img.shields.io/github/v/release/ucomesdag/ansible-role-bootstrap?include_prereleases&label=Release
[license-badge]: https://img.shields.io/github/license/ucomesdag/ansible-role-bootstrap?label=License
[galaxy-badge]: https://img.shields.io/badge/Ansible-Galaxy-blue?style=flat&logo=ansible&logoColor=white&color=5bbcbf
[download-badge]: https://img.shields.io/ansible/role/d/ucomesdag/bootstrap?label=Role%20Downloads

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

bootstrap_timeout: 5
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
|almalinux      |latest, 8                |
|alpine         |latest, edge             |
|amazonlinux    |latest                   |
|archlinux      |latest                   |
|centos         |latest, stream8          |
|debian         |latest, buster           |
|fedora         |latest, rawhide, 34, 33  |
|opensuse       |latest                   |
|rhel           |latest, ubi8             |
|rocky          |latest, 8                |
|rpi-os         |latest                   |
|ubuntu         |latest, jammy, bionic    |

The minimum version of Ansible required is 2.16, tests have been done to:

- The previous version (2.16).
- The current version (2.17).
- ~~The development version (2.18 is unreleased).~~

See the [Ansible community changelogs](https://docs.ansible.com/ansible/devel/reference_appendices/release_and_maintenance.html#ansible-community-changelogs) for details.

## [Exceptions](#exceptions)

Some variations of the build matrix do not work. These are the variations and reasons why the build won't work:

| variation | reason                                                                                      |
|-----------|---------------------------------------------------------------------------------------------|
| py.*-2.17 | Ansible 2.17 requires python 3.8 or newer and will fail run on systems with older versions. |

If you find issues, please register them in [GitHub](https://github.com/ucomesdag/ansible-role-bootstrap/issues)

## [License](#license)

Apache-2.0
