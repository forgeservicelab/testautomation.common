
Test Automation
---------------

This repository includes common library used in other test automation script.

Preconditions
-------------

Client running these test need. For installing these there is a Ansible playbook at public git (https://git.forgeservicelab.fi/ansible-roles/robot_framework)

+ Robot Framwork
+ Selenium2Framwork library
+ Browser

Variables
---------

+ assets/secrets.txt Credentials used in testing
+ assets/resource.txt Browser to be used in testing etc...  
+ assets/environment_xxx.txt URLs to tested service


To encrypt secrets file:
    
    openssl des3 -in secrets.txt -out secrets.txt.crypted 

To decrypt secrets file:

    openssl des3 -d < secrets.txt.crypted > secrets.txt -k <password>

