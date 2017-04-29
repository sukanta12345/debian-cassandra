Debian-Cassandra
================

The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

cassandra_gpg_key_id: F758CE318D77295D
cassandra_series_version: 11x

cassandra_cluster_name: 'Test Cluster'
cassandra_listen_address: 'localhost' # blank, or 0.0.0.0
cassandra_rpc_address: 'localhost' # blank, or 0.0.0.0
cassandra_rpc_port: 9160

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-cassandra, cassandra_gpg_key_id: F758CE318D77295D, cassandra_series_version: 11x, , cassandra_cluster_name: 'Test Cluster', cassandra_listen_address: 'localhost' # blank, or 0.0.0.0, cassandra_rpc_address: 'localhost' # blank, or 0.0.0.0, cassandra_rpc_port: 9160 }

Tasks
-----

  - Install [Cassandra](http://cassandra.apache.org/)

License
-------

BSD
