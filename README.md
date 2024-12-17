k3s
=========

Role to install k3s ready for other apps to be added.

Requirements
------------

Linux box built with internet access and root access.

Role Variables with Defaults
--------------

```yaml
k3s_ulb_dir: /usr/local/bin
k3s_images: https://github.com/k3s-io/k3s/releases/download/v1.31.3%2Bk3s1/k3s-airgap-images-amd64.tar
k3s_binary: https://github.com/k3s-io/k3s/releases/download/v1.31.3%2Bk3s1/k3s
k3s_install: https://get.k3s.io/
k3s_rpm: https://github.com/k3s-io/k3s-selinux/releases/download/v1.6.latest.1/k3s-selinux-1.6-1.el9.noarch.rpm
k3s_root_dir: /root/k3s
k3s_install_file: install.sh
```

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
