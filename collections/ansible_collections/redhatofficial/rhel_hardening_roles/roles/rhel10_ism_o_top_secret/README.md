Australian Cyber Security Centre (ACSC) ISM Official - Top Secret
=========

Ansible Role for Australian Cyber Security Centre (ACSC) ISM Official - Top Secret  
  
Profile Description:  
This profile contains configuration checks for Red Hat Enterprise Linux 10  
that align to the Australian Cyber Security Centre (ACSC) Information Security Manual (ISM).  
The ISM uses a risk-based approach to cyber security. This profile provides a guide to aligning  
Red Hat Enterprise Linux security controls with the ISM, which can be used to select controls  
specific to an organisation's security posture and risk profile.  
A copy of the ISM can be found at the ACSC website:  
https://www.cyber.gov.au/ism

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
         - { role: redhatofficial.rhel_hardening_roles.rhel10_ism_o_top_secret }

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
