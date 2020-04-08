Folding At Home
===============

This is a very basic role to help get a simple instance of the Folding@home
client onto a bunch of servers.

Role Variables
--------------

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| fah_gpu        | false         | Enable/Disable GPU support |
| fah_power      | 'medium'      | Folding@Home power setting |
| fah_team       | 245681        | User team, defaults to HappyMushrooms |
| fah_user       | 'anonymous'   | Username |
| fah_passkey    | ""            | Password for registered users |
| fah_allow_ips  |  []           | Whitelist IPs allowed to access web client on port 7396 |
| fah_slots      | ['CPU']       | Define FAH slots |
| fah_state      | 'present'     | Install/uninstall fah client |


Dependencies
------------

N/A

Example Playbook
----------------

```
- hosts: all
  roles:
    - paulfantom.folding_at_home
```

License
-------

MIT
