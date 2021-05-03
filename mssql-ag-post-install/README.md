Role Name
=========

Role (mssql-post-install) is to set the SQL Server Configuration to the desired state on Windows hosts, based on InComm's defined standards & Microsoft best practices.

Pre-Requirements

------------
https://wiki.incomm.com/display/OPSDBA/Configuring+Ansible+Host+Node+for+Windows?src=contextnavpagetreemode

Role Variables
--------------
For a detailed list of role variables, refer to below url. 
https://wiki.incomm.com/display/OPSDBA/Deploying+MSSQL+Post+Install+Role+using+Ansible?src=contextnavpagetreemode

 
Dependencies
------------

No other roles are dependent on this role.

Example Playbook
----------------

Please refer to below link for detailed instructions.
https://wiki.incomm.com/display/OPSDBA/Deploying+MSSQL+Post+Install+Role+using+Ansible?src=contextnavpagetreemode

-- Check Mode
Ex 1: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -C
Ex 2: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -l sqldbt -C
Ex 3: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-qa-hosts -C

-- Check Mode with verbose
Ex 1: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -C -vvv
Ex 2: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -l sqldbt -C -vvv
Ex 3: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-qa-hosts -C -vvv

-- Execute Mode
Ex 1: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts
Ex 2: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -l sqldbt
Ex 3: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-qa-hosts

-- Execute Mode with specific tags
Ex 1: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts --tags "check_sqlagentsvc_exists"
Ex 2: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-dev-hosts -l sqldbt --tags "check_sqlagentsvc_exists"
Ex 3: ansible-playbook mssql-post-install.yml --ask-vault-pass  -i mssql-qa-hosts --tags "check_sqlagentsvc_exists"



License
-------

BSD

Author Information
------------------

Chandra Pothina
