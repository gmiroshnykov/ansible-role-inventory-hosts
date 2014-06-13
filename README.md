inventory-hosts
===============

This Ansible role adds all hosts from Ansible inventory to target's `/etc/hosts`.


Role Variables
--------------

    inventory_hosts:
      interface: eth0   # get IP address from this network interface
      localhosts: []    # extra list of localhost aliases to associate with '127.0.0.1'
      aliases: []       # extra list of hostname aliases to save


Example configuration
---------------------

inventory_hosts:
  interface: eth0
  localhosts: ['www.example.com', 'ftp.example.com']
  aliases:
    - name: example.net
      ip:   8.8.8.8
    - name: www.example.net
      ip:   8.8.8.8


License
-------

BSD


Author Information
------------------

George Miroshnykov <george.miroshnykov@gmail.com>
