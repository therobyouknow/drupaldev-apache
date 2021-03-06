#DrupalDev apache

[![Build Status](http://r2.ayil.co.uk:8080/buildStatus/icon?job=drupaldev-apache-dev)](http://r2.ayil.co.uk:8080/job/drupaldev-apache-dev/)

Modified vagrant config from puphpet. Supports Drupal 6/7/8. Built in Drush and Composer.

#DrupalDev Nginx

Please consider using https://github.com/mikebell/drupaldev-nginx instead, this is barely maintained and various issues means that updating it has become impossible. If anyone wants to maintain this then please fork.

#Tools
1. Removed xhprof it doesn't work in this config
2. Easier handling of vhosts and dbs (see example.pp)
3. Drush
4. Compass
5. Omega 4 Gems included as standard
6. APC / Memcache
7. Mailcatcher - access example.drupal.dev:1080

#Dependencies
* Xcode with Command Line Tools installed
* Vagrant - http://www.vagrantup.com/
* VirtualBox - https://www.virtualbox.org/

#Install

1. Clone Me
2. `cd drupaldev-apache`
3. `mkdir sites`
4. `cp manifests/example.pp manifests/devsites.pp`
5. Amend manifests/devsites.pp as required to desired server/virtualhost name and db details
6. `vagrant up`

#VM Info
* Default port 33.33.33.10
* Sites built as *.drupal.dev (use dnsmasq)
* Ubuntu 12.04

