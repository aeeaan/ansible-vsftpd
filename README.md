correct.horse.vsftpd
=========

This role is for a very basic install of vsftpd. The primary focus of this role is running an ftp server on localhost for upgrading a wordpress install. For increased security, wordpress shouldn't have write access to anything other than upload and cache directories. The localhost ftp site allows wordpress and its plugins to still be upgraded via the admin site.

Role Variables
--------------

TODO

Dependencies
------------

TODO

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correct.horse.vsftpd }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
