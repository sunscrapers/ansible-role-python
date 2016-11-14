# Ansible Python role

Ansible Python roles installs Python ubuntu packages including development headers. If specified it also installs pip,
setuptools and virtualenv or just update these packages to latest versions.

Developed by [SUNSCRAPERS](http://sunscrapers.com/) with passion & patience.

## Customization

To customize the role you can override the following default variables:

```yaml
python_install_2: yes
python_apt_packages_2:
  - python
  - python-dev
  - python-pip

python_install_3: yes
python_apt_packages_3:
  - python
  - python-dev
  - python-pip

python_pip_packages: []

python_update_pip: no
python_update_setuptools: no
python_install_virtualenv: no

python_pip_executable:
# python_pip_version:           # default to latest
# python_setuptools_version:    # default to latest
# python_virtualenv_version:    # default to latest
```

## Development

To start developing on this Ansible role you need to install [Vagrant](https://www.vagrantup.com/) first. Then run:

```
$ vagrant up
```

to start and provision virtual machine. You can run provisioning again to test idempotence:

```
$ vagrant provision
```
