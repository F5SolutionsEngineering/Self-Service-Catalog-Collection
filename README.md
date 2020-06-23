# SScatalog_collection
This repo contains an Ansible Galaxy collection for SSportal targeted use cases.
<MORE>

## Supporting documentation
["Developing Collections" Documentation](https://docs.ansible.com/ansible/latest/dev_guide/developing_collections.html) 

## Directory Structure
Roles in this repository should follow the Ansible role directory structure standard. 
```shell
.
collection/
├── docs/
├── galaxy.yml
├── plugins/
│   ├── modules/
│   │   └── module1.py
│   ├── inventory/
│   └── .../
├── README.md
├── roles/
│   ├── role1/
│   ├── role2/
│   └── .../
├── playbooks/
│   ├── files/
│   ├── vars/
│   ├── templates/
│   └── tasks/
└── tests/
```

## Referencing the Collection
For Ansible 2.9 the following can be used in ``requirements.yml``:

```yaml
---
collections:
- name: 'https://github.com/F5SolutionsEngineering/Self-Service-Catalog-Collection/releases/<<MORE>>'
```

The collection namespace, as determined by ``galaxy.yml``, will be "ss-cat".

## Contribution Guidelines
Please feel free to add functionality to this collection for your customer's use case.
If you'd like assistance, contact the repo maintainers or create an issue.

Contributors should fork or create a branch depending on thier user permissions.
Contributions should be made through pull requests which will then be approved by one or more maintainers.

## Building the Collection
<<instructions on galaxy build commands>>

## Included Roles
Roles included in this collection should be documented in this section.

### ipam-infoblox

### ipam-phpipam

### bigip-as3-deploy

### cert-cfssl

## Roles under development

### cert-acme-bigip

## Future Roles

### Essential App Protect

### BIG-IP DNS GSLB

### F5CS GSLB

## TBD

### Attributions
- The `ipam-phpipam` role is a derivative of the [ansible_mod-phpIPAM](https://github.com/rcanderson23/ansible_mod-phpIPAM) repository. I've repackaged the code into a more standard role directory. Additional modifications will be tracked here.


