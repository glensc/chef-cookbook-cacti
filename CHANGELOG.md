## 0.3.0

* DEPRECATED: server recipe; use default recipe or individual recipes as needed
* Enhancement: Chef solo support for unencrypted data bags
* Enhancement: Fallback to new `node['cacti']['admin']` and `node['cacti']['database']` attributes if no data bag (now easily Vagrant testable)
* Enhancement: Fedora 19 and 20 support
* Enhancement: Ubuntu 12.10, 13.04, and 13.10 support
* Enhancement: Migrate apache2 configuration in server recipe to apache2 recipe
* Enhancement: Migrate cron configuration in server recipe to cron recipe
* Enhancement: Migrate configuration in server recipe to configuration recipe
* Enhancement: Migrate database configuration in server recipe to database recipe
* Enhancement: Migrate package installation in server recipe to package recipe
* Enhancement: Move hardcoded packages in recipes into `node['cacti']['packages']` and `node['cacti']['spine']['packages']` attributes (/ht @stormerider)
* Enhancement: Move dbconfig and poller in server recipe into `node['cacti']['db_file']` and `node['cacti']['poller_file']` attributes
* Enhancement: Add `node['cacti']['rrdtool']['version']` to help with default platform package versioning in database
* Enhancement: Auto-detect default cacti package version per Ubuntu release
* Enhancement: Default recipe installs EPEL for RHEL family OSes

## 0.2.0

* Add Ubuntu support (thanks @stormerider!)

## v0.1.1

* Fixed spine copying to perserve mode and ownership
* Added php-ldap to server recipe packages list

## v0.1.0

* Initial release.
