What's ELRyu
============
ELRyu is a component-based software defined networking framework, based on Ryu.

Ryu provides software components with well defined API that make it
easy for developers to create new network management and control
applications. Ryu supports various protocols for managing network
devices, such as OpenFlow, Netconf, OF-config, etc. About OpenFlow,
Ryu supports fully 1.0, 1.2, 1.3, 1.4, 1.5 and Nicira Extensions.

All of the code is freely available under the Apache 2.0 license. ELRyu
is fully written in Python3 based on Ryu.


Quick Start
===========
Installing Ryu is quite easy::

   % git clone git://github.com/elahejalalpour/elryu.git
   % cd ryu; python3 ./setup.py install

If you want to use Ryu with `OpenStack <http://openstack.org/>`_,
please refer `networking-ofagent project <https://github.com/stackforge/networking-ofagent>`_.

If you want to write your Ryu application, have a look at
`Writing ryu application <http://ryu.readthedocs.org/en/latest/writing_ryu_app.html>`_ document.
After writing your application, just type::

   % ryu-manager your_app.py


Optional Requirements
=====================

Some functionalities of ryu requires extra packages:

- OF-Config requires lxml
- NETCONF requires paramiko
- BGP speaker (ssh console) requires paramiko

If you want to use the functionalities, please install requirements::

    % pip install lxml
    % pip install paramiko


Ryu Support
===========
Ryu Official site is `<http://osrg.github.io/ryu/>`_.

If you have any
questions, suggestions, and patches, the mailing list is available at
`ryu-devel ML
<https://lists.sourceforge.net/lists/listinfo/ryu-devel>`_.
`The ML archive at Gmane <http://dir.gmane.org/gmane.network.ryu.devel>`_
is also available.
