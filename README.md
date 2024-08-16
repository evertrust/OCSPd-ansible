Role Name
=========

This role deploys OCSPd on a VM running on RH8 and restores a backup file on this new instance. 


Requirements
------------

For the process to work properly, it is necessary that these requirements are met before using the role : 

| Control node        | Host   |
|---------------------|--------|
| active licence      | ocspd-3.1.3.noarch.rpm |
| root access to host | backup file |
 

The IP address / DNS Name of one or several NTP server(s);

The IP address / DNS Name of an SMTP relay;

The email address of the OCSPd server administrator.

Flows for services https and http opened.



Role Variables
--------------

You will find 2 variable sets in this role under OCSP/defaults/main/.
All the variables in mandatory_vars.yml must be set prior to using the role and match your environment. 
The ones in default_values.yml are optional and can be changed after the backup process if needed.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
    
    - name: testPlaybook
      hosts: all
      roles:
        - role: OCSP
          tags: always



Author Information
------------------

If you got any question or ideas concerning this role, please contact Evertrust. 