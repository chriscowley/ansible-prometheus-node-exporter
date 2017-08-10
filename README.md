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

| Variable                                      | Required | Default   | Choices     | Comments                                    |
|-----------------------------------------------|----------|-----------|-------------|---------------------------------------------|
| PROMETHEUS_NODE_EXPORTER_MONITOR_RAID_STORCLI | no       | false     | true, false | Monitor RAID with StorCLI                   |
| PROMETHEUS_NODE_EXPORTER_CUSTOM_OPTS          | no       | undefined | string      | Additional options to pass to node_exporter |

Dependencies
------------

If `PROMETHEUS_NODE_EXPORTER_MONITOR_RAID_STORCLI` is set, storcli must be installed a la https://gitlab.cyverse.org/config-mgmt/ansible-install-storcli

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
