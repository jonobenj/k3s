k3s
=========

Role to install k3s ready for other apps to be added.

Requirements
------------

Linux box built with internet access and root access.

Role Variables
--------------



Example Playbook
----------------

```yaml
    - name: Install k3s
      hosts: all
      ansible.builtin.include_role:
        name: k3s
        apply:
          become: true
```

License
-------

BSD

Author Information
------------------

Fen UwU
