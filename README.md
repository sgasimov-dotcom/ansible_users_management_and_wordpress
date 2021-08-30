Role Description
=========


------------

This Role was created for my class Project. Taks requirements were the following:


- Please create an ansible role that installs WordPress on Operating systems. 

- The same role should add 5 users with ssh keys generated on ubuntu machines, and add those users to a devops group.

- Those users should have root privileges.

- For testing purposes this role should install telnet for future use. 
- Once the role is created, please publish on galaxy.ansible.com by utilizing the following documentation

- https://opcitotechnologies.medium.com/how-to-write-ansible-roles-and-publish-them-on-ansible-galaxy-e750cd457619#:~:text=Ansible%20Galaxy%20is%20Ansible's%20official,known%20to%20Ansible%20as%20Roles.

- https://galaxy.ansible.com/docs/contributing/index.html
--------------


1 - Wordpress on Ubuntu 20.04 LAMP
------------------


This playbook will install a WordPress website on top of a LAMP environment (**L**inux, **A**pache, **M**ySQL and **P**HP) on an Ubuntu 18.04 machine. A virtualhost will be created with the options specified in the `vars/default.yml` variable file.


## Settings

- `php_modules`:  An array containing PHP extensions that should be installed to support your WordPress setup. You don't need to change this variable, but you might want to include new extensions to the list if your specific setup requires it.
- `mysql_root_password`: The desired password for the **root** MySQL account.
- `mysql_db`: The name of the MySQL database that should be created for WordPress.
- `mysql_user`: The name of the MySQL user that should be created for WordPress.
- `mysql_password`: The password for the new MySQL user.
- `http_host`: Your domain name.
- `http_conf`: The name of the configuration file that will be created within Apache.
- `http_port`: HTTP port for this virtual host, where `80` is the default. 

----------------


2 - Users and Groups Management
------------------
------------

This role  will create users and groups.

Run playbook: `ansible-playbook playbooktask2.yaml` 

Variables are located in: users_groups/vars.yml variable file.



-------

