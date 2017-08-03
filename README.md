prometheus-node-exporter
=========

Deploys the Node Exporter for Prometheus.

[![Build Status](https://travis-ci.org/CyVerse-Ansible/ansible-prometheus-node-exporter.svg?branch=master)](https://travis-ci.org/CyVerse-Ansible/ansible-prometheus-node-exporter)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-prometheus--node--exporter-blue.svg)](https://galaxy.ansible.com/CyVerse-Ansible/prometheus-node-exporter/)


Requirements
------------

None

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

| Variable                              | Required | Default   | Choices     | Comments                                    |
|---------------------------------------|----------|-----------|-------------|---------------------------------------------|
| PROMETHEUS_NODE_EXPORTER_MONITOR_RAID | no       | false     | true, false | Monitor RAID with MegaCLI                   |
| PROMETHEUS_NODE_EXPORTER_CUSTOM_OPTS  | no       | undefined | string      | Additional options to pass to node_exporter |

Dependencies
------------

None, but monitor_raid option designed to work with https://gitlab.cyverse.org/config-mgmt/ansible-install-megacli

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - prometheus-node-exporter

License
-------

See license.md

Author Information
------------------

https://cyverse.org
