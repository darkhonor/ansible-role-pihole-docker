# Ansible Role to Install Pi-Hole on Docker

This role will setup [Pi-Hole](https://pi-hole.net/) running as a [Docker Container](https://hub.docker.com/).
This role takes a good portion of the setup from Sebastian Haderecker's [ansible-pihole](https://github.com/shaderecker/ansible-pihole)
role.  I've adjusted to meet some additional security and system-level customization.  This is a preference and where
possible, I've added boolean flags in the `defaults\main.yml` file to allow you to customize your experience.

## Requirements

This role assumes you've already setup the system with Docker.  I've made my docker role as a dependency.

## Role Variables

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

## Dependencies

The following roles are required:

* [darkhonor.docker](https://galaxy.ansible.com/darkhonor/docker)

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

## License

MIT

## Author Information

Alex Ackerman, X @darkhonor
