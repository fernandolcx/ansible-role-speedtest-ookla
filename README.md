ansible-role-speedtest-ookla
==========================

Ansible role that deploys and configure [Ookla](https://www.speedtest.net/) speedtest server. Apache with PHP is required and is installed automatically.

You can find original installation steps at https://support.ookla.com/hc/en-us/articles/234578528

The service listens on 5060 and 8080.

You can validate your server at https://www.ookla.com/host-tester

You can register your server at https://account.ookla.com/register/servers.

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
    - fernandolcx.ookla_speedtest
```

Run with:

```
ansible-playbook -i "192.168.0.100:29019," speedtest.yml -u myuser --ask-pass --become --ask-become-pass
```



Author information
------------------

[Solustic](http://www.solustic.com.br/) - Soluções em tecnologia - 2021