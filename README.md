ACCESS - ssh
=========

Configure SSH and exchange public and host keys.

Requirements
------------

SSH server to be installed on target hosts

Role Variables
--------------

| Variable                 | Description                                                               | Default           |
|--------------------------|---------------------------------------------------------------------------|-------------------|
| ssh_admin_key            | Path to public key on local machine to be authorized on target host       | ~/.ssh/id_rsa.pub |
| ssh_enable_internode_ssh | Enable password-less SSH from every target host to every other target host | False             |

Refer to the defaults for other customizable SSH settings

Dependencies
------------

None

Example Playbook
----------------
```yaml
- hosts: all
  roles:
  - access_ssh_keys
```

License
-------
BSD

Author Information
------------------
jakoberpf
