Ansible Role: OpenStack Nova Controller
=======================================

This role installs and configures OpenStack Nova Compute Node on EL7 system.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`)

    host: controller

Host that runs Nova services.

    ip_address:

IP address in management network.

    keystone_host: controller
    keystone_password:

Keystone credentials for Nova user.

    keystone_admin_password:

Password for admin Keystone user.

    mysql_host: controller
    mysql_password:

MySQL credentials.

    rabbitmq_host: controller
    rabbitmq_user:
    rabbitmq_password:

RabbitMQ credentials.

    glance_host: controller

Glance API host.

    region: RegionOne

OpenStack region.

    neutron_host: controller
    neutron_password:

Neutron credentials.

    metadata_secret:

Secret token for metadata proxy.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - binarycode.openstack-nova-controller

License
-------

BSD

Author Information
------------------

[Igor Sidorov](https://github.com/binarycode)
