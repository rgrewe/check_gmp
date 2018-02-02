=========================
GMP Nagios Command Plugin
=========================

.. contents:: Table of contents

Introduction
~~~~~~~~~~~

*check_gmp* is a plugin for nagios or similar systems. It communicates with a Greenbone Security Manager and retrieve vulnerability data of specific hosts. These data are saved in reports. For better performance check_gmp saves the generated reports from the gsm in a sqlite database. 

Requirements
~~~~~~~~~~~
- `gvm-tools`_

.. _gvm-tools: https://github.com/greenbone/gvm-tools
.. Python3

Installing
~~~~~~~~~~

To install it, after downloading the repository, you have to copy check_gmp.py into the nagios plugin directory.

On Debian Linux Systems::

    /usr/lib/nagios/plugins

Otherwise to test the script without nagios, you can execute it directly with::
    
    $ python3 check_gmp.py ssh -H host -u user -w pass --ping

Command parameter
~~~~~~~~~~~~~~~~
There are several command parameter. Some of them will be explained in detail in future.
