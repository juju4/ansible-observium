[![Build Status](https://travis-ci.org/juju4/ansible-observium.svg?branch=master)](https://travis-ci.org/juju4/ansible-observium)
# Observium ansible role

A simple ansible role to setup observium community
http://www.observium.org/

## Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 1.9
 * 2.0

### Operating systems

Tested with vagrant on Ubuntu 14.04, Kitchen test with trusty and centos7

## Example Playbook

Just include this role in your list.
For example

```
- host: all
  roles:
    - observium
```

Currently works with recommended setup including mysql, apache2

## Variables

Nothing specific for now.

## Continuous integration

This role has a travis basic test (for github), more advanced with kitchen and also a Vagrantfile (test/vagrant).

Once you ensured all necessary roles are present, You can test with:
```
$ cd /path/to/roles/observium
$ kitchen verify
$ kitchen login
```
or
```
$ cd /path/to/roles/observium/test/vagrant
$ vagrant up
$ vagrant ssh
```

## Troubleshooting & Known issues


## License

BSD 2-clause

