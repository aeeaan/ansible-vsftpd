correcthorse.vsftpd
=========

This role is for a very basic install of vsftpd. 

Role Variables
--------------
| Variable				| Default				| Notes					|
| :---					| :---					| :---					|
| vsftpd_anonymous_enable		| false					|					|
| vsftpd_local_enable			| true					|					|
| vsftpd_virtual_users			| true					|					|
| vsftpd_virtual_user_db		| /etc/vsftpd/vsftpd_login		|					|
| vsftpd_virtual_root			| /var/ftp				|					|
| vsftpd_virtual_root_owner		| ftp					|					|
| vsftpd_virtual_root_group		| ftp					|					|
| vsftpd_user_sub_token			| $USER					|					|
| vsftpd_chroot_local_user		| true					|					|
| vsftpd_listen_ipv6			| false					|					|
| vsftpd_listen_address			| 127.0.0.1				|					|
| vsftpd_listen_address6		| "::1"					|					|
| vsftpd_pasv_enable			| true					|					|
| vsftpd_pasv_min_port			| 1024					|					|
| vsftpd_pasv_max_port			| 1048					|					|
| vsftpd_pasv_address			| ''					|					|
| vsftpd_ssl_enable			| false					|					|
| vsftpd_rsa_cert_file			| ''					|					|
| vsftpd_rsa_private_key_file		| ''					|					|
| vsftpd_allow_anon_ssl			| true					|					|
| vsftpd_force_local_data_ssl		| true					|					|
| vsftpd_force_local_logins_ssl		| true					|					|
| vsftpd_ssl_tlsv1			| true					|					|
| vsftpd_ssl_sslv2			| false					|					|
| vsftpd_ssl_sslv3			| false					|					|
| vsftpd_ssl_request_cert		| false					|					|
| vsftpd_validate_cert			| false					|					|
| vsftpd_require_ssl_reuse		| false					|					|
| vsftpd_ssl_ciphers			| HIGH					|					|

Dependencies
------------

- correcthorse.common

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.vsftpd }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
