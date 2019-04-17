Role Name
=========

This role update the DNS forward and reverse zone files

Requirements
------------

Need to have DNS and bind-utils installed

Must supply following variables:
    zone: example.com
    zone_file: db.example.com
    ipaddress: 172.18.10.212
    hostname: webserver
    ptr_zone: 10.18.172.in-addr.arpa
    ptr_zone_file: db.10.18.172.in-addr.arpa

License
-------

BSD
No warranty

Author Information
------------------
Eric Chong
