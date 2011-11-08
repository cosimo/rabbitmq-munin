=========================
 RabbitMQ Munin Plug-Ins
=========================

Monitor RabbitMQ in your environments.

Installation
============

Copy the plug-ins to the munin plugin directory, e.g ``/etc/munin/plugins/``.

Granting Permissions
====================

To use these plug-ins you have to tell munin-node to execute them as
root by changing the plug-in configuration file (on debian that is
``/etc/munin/plugin-conf.d``)::

    [rabbitmq-*]
    user root

Using a Custom Virtual Host
============================

You can set the name of virtual host by changing the plug-in configuration
file (on debian that is ``/etc/munin/plugin-conf.d``)::

    [rabbitmq-*]
    env.vhost vhostname

Author
======

Ask Solem <askh@opera.com>
Brad Gessler <opensource@polleverywhere.com>