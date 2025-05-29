Role Name
=========
nginx  

Requirements
------------

This role installs and configures NGINX on Ubuntu servers. It also installs curl and git, and deploys a custom HTML page.
Role Variables
--------------
- `nginx_packages`: List of packages to install (default: nginx, curl, git)
Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

TO RUN ALL  # ansible-playbook -i inventory.ini webserver-playbook.yml

TO RUN USING SPECIFIC PART USING TAGS 
 - TO INSTALL PACKAGES  # ansible-playbook -i inventory.ini webserver-playbook.yml --tags "install"

 - TO COPY HTML FILE # ansible-playbook -i inventory.ini webserver-playbook.yml --tags "copy"

 - TO START OR  ENABLE NGINX # ansible-playbook -i inventory.ini webserver-playbook.yml --tags "service"

 - TO creare user only # ansible-playbook -i inventory.ini webserver-playbook.yml --tags "user" 






