Australian Cyber Security Centre (ACSC) Essential Eight
=========

Ansible Role for Australian Cyber Security Centre (ACSC) Essential Eight  
  
Profile Description:  
This profile contains configuration checks for Red Hat Enterprise Linux 8  
that align to the Australian Cyber Security Centre (ACSC) Essential Eight.  
A copy of the Essential Eight in Linux Environments guide can be found at the  
ACSC website:  
https://www.cyber.gov.au/acsc/view-all-content/publications/hardening-linux-workstations-and-servers

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing in this role,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

Requirements
------------

- Ansible version 2.9 or higher

Role Variables
--------------

To customize the role to your liking, check out the `defaults/main.yml`.

Dependencies
------------

N/A

Example Role Usage
----------------

Install the `redhatofficial.rhel_hardening_roles` collection, then use the following playbook snippet:

    - hosts: all
      roles:
         - { role: redhatofficial.rhel_hardening_roles.rhel8_e8 }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

License
-------

BSD-3-Clause

Author Information
------------------

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
