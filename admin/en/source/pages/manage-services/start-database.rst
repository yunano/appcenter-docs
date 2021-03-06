.. Copyright 2016 FUJITSU LIMITED

.. _start-database:

Starting and Stopping the Database
----------------------------------

The database is registered as an operating system service. Each time a database node is rebooted, MariaDB is restarted automatically as part of the node boot sequence. To manually stop or start the database you must be the unix root user of the node. Log in to the database node as root::

  $ ssh root@<ip address of the node>

Stopping the Database
~~~~~~~~~~~~~~~~~~~~~

.. code-block:: shell

  $ service mysql stop

Starting the Database
~~~~~~~~~~~~~~~~~~~~~

.. code-block:: shell

  $ service mysql start

Restarting the Database
~~~~~~~~~~~~~~~~~~~~~~~

.. code-block:: shell

  $ service mysql restart
