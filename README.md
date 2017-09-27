Role Name
=========

This role installs and configures oracle-xe on linux platforms.

Requirements
------------

You must accept the license agreement, download oracle-xe-11.2.0-1.0.x86_64.rpm.zip (for the linux x64 platform), and copy it to the playbook directory or to the files directory within this role from:

http://www.oracle.com/technetwork/database/database-technologies/express-edition/downloads/index.html

Alternatively, you can define the var oracle_xe_archive_url in tasks/main.yml to download the RPM as part of the play

Role Variables
--------------

- oracle_http_port: 8080
- oracle_listener_port: 1521
- oracle_password: manager
- oracle_dbenable: y
- oracle_xe_archive_url: if this url is defined, the role will attempt to download the above zip file from it.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
