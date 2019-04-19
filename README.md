### This is an exmaple of configuring zone files with Ansible

Example 02-add_record_by_nsupdate.yml uses nsupdate to update dynamic DNS

Example 04-add_record_by_role.yml uses the attached role to update the zone files.

Example
-------

```yaml
---
- name: Update forward and reverse zone files
  hosts: localhost
  connection: smart
  gather_facts: no

  vars:
    zone: dev.iisl.com
    zone_file: db.dev.iisl.com
    ipaddress: 172.18.10.212
    hostname: dummy2
    ptr_zone: 10.18.172.in-addr.arpa
    ptr_zone_file: db.10.18.172.in-addr.arpa


  roles:
  - update_zone
```
