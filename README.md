Longhorn
=========

Install [Longhorn](https://longhorn.io/) storage on Kubernetes cluster

Requirements
------------

* Kubernetes cluster that supports LoadBalancer service which is required by the Longhorn web frontend provisioned by this role
* ```KUBECONFIG``` configured and present on Ansible controller host

Role Variables
--------------

* ```longhorn_ui_ip``` - IP address for Longhorn web frontend

Example Playbook
----------------

    - hosts: servers
      environment:
        KUBECONFIG: /path/to/your/kubeconfig/on/ansible/controller
      roles:
        - role: krittin.longhorn
          longhorn_ui_ip: 10.10.1.1


License
-------

MIT

