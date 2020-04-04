# Install

This set of playbooks have specific dependencies on Ansible due to the modules being used.

## Ansible Molecule

### Requirements

- Ansible 2.9
- Docker
- docker-py

### Install OS Dependencies on CentOS 8 for Ansible Molecule

```
sudo yum install -y gcc python3-pip python3-devel openssl-devel libselinux-python

# Molecule from source
sudo yum install libffi-devel git
```

### Install OS dependencies on Ubuntu 16.x for Ansible Molecule

```
$ sudo apt-get update
$ sudo apt-get install -y python3-pip libssl-dev

# From source
$ sudo apt-get install -y libffi-dev git
```

### Install OS dependencies on MacOS for Ansible Molecule

```
$ brew install python git
```

### Install Ansible Molecule

For more information: https://molecule.readthedocs.io/en/latest/installation.html

```
$ python3 -m pip install --upgrade --user setuptools
$ python3 -m pip install --user "molecule[lint]"

# From source
$ python3 -m pip install -U git+https://github.com/ansible-community/molecule
```

## Ansible for Kubernetes

### Requirements

```
$ pip install openshift kubernetes
```
