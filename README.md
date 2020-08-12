ansible-role-speedtest-ookla
==========================

Ansible role that deploys and configure [Ookla](https://www.speedtest.net/) speedtest server. Apache with PHP is required and is installed automatically.

You can find original installation steps at https://support.ookla.com/hc/en-us/articles/234578528

The service listens on 5060 and 8080.

You can validate your server at https://www.ookla.com/host-tester

Requirements
------------

* Debian 9 or newer
* Ubuntu 18.04 or newer

Role Variables
--------------

```yaml
ookla_directory: /opt/ookla
```

Example Playbook
----------------

```yaml
- name: Install Ookla speedtest server
  hosts: all
  become: yes
  roles:
    - ansible-role-speedtest-ookla
```

Author information
------------------

[Solustic](http://www.solustic.com.br/) - Soluções em tecnologia - 2020
