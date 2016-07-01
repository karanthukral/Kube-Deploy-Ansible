kube-deploy
=========

Ansible role to install docker and deploy kubernetes on an Ubuntu cluster. The deployment uses docker to run the required kubernetes components. The install script can be found at [docker-multinode](https://github.com/kubernetes/kube-deploy/tree/master/docker-multinode)

Requirements
------------

This role currently only supports ubuntu.

Role Variables
--------------

`master_ip` is required by the role to ensure the correct components are installed on the master node vs the worker node.

Dependencies
------------
This role does not have any dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
---
- vars:
    master_ip: 64.x.x.x
  hosts: kube-cluster

  roles:
    - kube-deploy
```


License
-------

MIT
