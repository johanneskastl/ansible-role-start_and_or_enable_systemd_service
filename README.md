![Ansible Lint](https://github.com/johanneskastl/ansible-role-start_and_or_enable_systemd_service/workflows/Ansible%20Lint/badge.svg)

start_and_or_enable_systemd_service
=========

Start and/or enable a systemd service.

Requirements
------------

None.

Role Variables
--------------

- `service_name`: Name of the service to be modified (Required).
- `service_started`: Set to `true` if the service should be started (Required).
- `service_enabled`: Set to `true` if the service should be enabled (Required).

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: 'johanneskastl.start_and_or_enable_systemd_service', service_name: 'sshd', service_started: 'True', service_enabled: 'True' }

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
