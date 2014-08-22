# enrise.apt

This is an Ansible task for making sure that your APT caches are up to date.

## Requirements

- Tested on Ansible 1.5
- Tested on Ubuntu 14.04 (trusty), but it should work on any modern Debian based system.

## Dependencies

None.

## Example playbook

This role is so terribly simple, only one variable exists.

    - hosts: all
      sudo: yes
      vars_files:
        - vars/apache.yml
      roles:
        - { role: enrise.apt, apt_cache_valid_time: 3600 }

## Licence

MIT

## Feedback? Found a bug? Requests?

That's special, considering this is a one-task role. But still: let us have it!
http://github.com/Enrise/ansible-role-apt/issues
