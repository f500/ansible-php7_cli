Deprecated
==========

**This role is deprecated. Please use the role [f500.php7](https://github.com/f500/ansible-php7), v1.0.0 or higher.**

---

PHP7_CLI
========

Install PHP cli


Requirements
------------

Debian Jessie with the package python-pycurl and python-software-properties installed.

Role Variables
--------------

There are as many role variables as PHP.ini variables. All of them can be set, but the defaults
are adjusted according to [iniscan](https://github.com/psecio/iniscan) security best practices.

This package depends on f500.php7, and all the php_* variables are used as defaults for the php_cli* variables.

Dependencies
------------

Depends on f500.php7.

Example Playbook
-------------------------

    - hosts: servers
      roles:
        - { role: f500.php7_cli, php_cli_error_reporting: "E_ALL" }

License
-------

Copyright (C) 2017 Future500 B.V.

[LGPL-3.0](https://github.com/f500/ansible-php7_cli/blob/master/COPYING.LESSER)

Author Information
------------------

Jasper N. Brouwer, jasper@future500.nl

Ramon de la Fuente, ramon@future500.nl
