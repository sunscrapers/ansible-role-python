# Ansible Python role

Ansible Python roles installs Python ubuntu packages including development headers. If specified it also installs pip,
setuptools and virtualenv or just update these packages to latest versions.

Developed by [SUNSCRAPERS](http://sunscrapers.com/) with passion & patience.

## Customization

To customize the role you can override the following default variables:

```yaml
python_apt_packages:
  - python
  - python-dev
  - python-pip
python_pip_packages: []
# python_pip_version:           # default to latest
# python_setuptools_version:    # default to latest
# python_virtualenv_version:    # default to latest
```

In order to install Python 3 as well customize variables like that:

```yaml
python_apt_packages:
  - python
  - python-pip
  - python-dev
  - python3
  - python3-pip
  - python3-dev
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
