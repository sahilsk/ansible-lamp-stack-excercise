README
--------

### Ansible role to setup lamp stack

- edit inventory file  (staging)
- edit playbook webservers.yml


### Downlaod galaxy modules

- personnage.php
- mstantoncook.mysql

	$ ansible-galaxy install <module-name>


### How-to-run
---


Test-connection
		
	ansible all -i staging -m ping

If all, ok, proceed further

	ansible-playbook webservers.yml -i staging


>NOTE: Passwords are hardcoded. Do, replace them or specify with environment variables

Todo
---

- php-fpm fix
