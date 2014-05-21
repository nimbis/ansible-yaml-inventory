ansible-yaml-inventory
======================

YAML inventory for Ansible.  

This looks for a hosts.yml file in the same directory as this executable.

File format:

```
- <hostname>
```

or

```
- host: <hostname>
  vars:
  - myvar: value
  - myvbr: vblue
  groups:
  - mygroup1
  - mygroup2
```
or

```
- group: <groupname>
  vars:
  - groupvar: value
  hosts:
  - myhost1
  - myhost2
  groups:
  - subgroup1
  - subgroup2
```

Any statement except the first definition is optional.
