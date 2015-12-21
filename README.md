# Vagrantfile + Puppet

Deploys Virtualbox locally to 192.168.56.101 (currently vagrant.dev in nginx conf)

Plays well with Laravel 5.

### Summary

- Ubuntu Trusty 14.04 LTS x64
- PHP (fpm) 5.6 with 
	- cli
    - intl
    - mcrypt
    - memcache
    - mbstring
    - curl
    - redis
- Nginx, MariaDB 10.1, Redis Server
- see ./puphpet/config.yaml

### .gitignore

If you're new to Vagrant, you might want to add this to your .gitignore to avoid
tracking vm instance files.

	# Vagrant/Puppet
	.vagrant
	puphpet/files/dot/ssh
	!puphpet/files/dot/ssh/insecure_private_key

	# TODO: remove this from manifest?
	html/index.html