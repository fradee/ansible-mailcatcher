# Ansible Role: Mailcatcher

Ansible playbook to install mailcatcher on Ubuntu Servers


## Requirements

None.

## Role Variables

Available variables are listed below with its default values.

set up mail catcher depend php version:

	mailcatcher_php_version: 5.6

enable mailcatcher as service:

    mailcatcher_startup_on_boot: true

## Dependencies

None. Works best with [geerlingguy.php](https://galaxy.ansible.com/geerlingguy/php/).

## Example Playbook

	---
	- hosts: all
	  user: vagrant
	  sudo: true
	  vars:
		  - mailcatcher_php_version: 7.0
		  - mailcatcher_startup_on_boot: true
	  roles:
		  - fradee.mailcatcher

## License

BSD

## Notes

It is a beta version and can be improved, please help me to improve and fix bugs for this playbook.

Thanks.
