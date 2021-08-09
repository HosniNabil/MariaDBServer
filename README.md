MariaDBServer
=========

MariaDB initial server configuration.

Role Variables
--------------
The required variables for this are :

- set_root_pw:  yes | no , in case the root password wasn't set before, this variable should be set to yes
- root_password: this varibale should contain the previously set root password
- new_root_password: new root password for the mariadb server
- sql_db: database name to be created
- sql_user: database admin username to be created
- sql_password: admin user password


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: mariadb_servers
      roles:
         - { role: hosninabil.mariadbserver, set_root_pw: yes, new_root_password: 'password', sql_db: newdb, sql_user: admin, sql_password: 'password' }

License
-------

Apache-2.0

Author Information
------------------

Nabil Hosni, cloud engineer and opensource enthusiast.
