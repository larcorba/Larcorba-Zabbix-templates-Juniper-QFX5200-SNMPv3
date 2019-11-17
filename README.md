Zabbix template
======

Intro
------
Check out Zabbix share and drop a rating/comment! :)

https://share.zabbix.com/network_devices/juniper/juniper-qfx5200-snmpv3


Features
------
- Interface discovery
  - Interface utilization and triggers
  - Optical dBm values
  - No more logical interfaces by default
- Hardware discovery + triggers
- BGP discovery + trigger
- Inventory


Macros
------
Do not forget the add the macro's:

User: {$JUN_V3_USER}

Password: {$JUN_V3_AUTHPASS}


Inventory
------
Make sure to add the inventory 'automatic' options at your host if you want to use the invetory option.

Logical interface disovery
------
^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+\.[0-9]+$|^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(reth|st)[0-9]+\.[0-9]+$|^(reth|st)[0-9]$|^vcp-[0-9]+$|^vlan.[0-9]+$

or

^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(fe|ge|xe|et)-[0-9]+\/[0-9]+\/[0-9]+$|^(reth|st)[0-9]+$|^(reth|st)[0-9]$|^vcp-[0-9]+$|^vlan.[0-9]+$
