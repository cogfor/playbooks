playbooks
=========

Playbooks for Cogfor infrastructure.

# Create wordpress site

ansible-playbook -i hosts/cog4-www site.yml -v --extra-vars "mysql_root_password=verysecretpassword wp_db_password=anothersecretpassword"

This will do a complete php5 installation, with nginx and php-fpm and varnish caching. Don't forget to specify the:

* mysql_root_password
* wp_db_password


