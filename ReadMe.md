# phpMyAdmin Database Management Utility for TYPO3

phpMyAdmin is a free software tool written in PHP, intended to handle the administration of MySQL over 
the Web. phpMyAdmin supports a wide range of operations on MySQL, MariaDB and Drizzle. Frequently 
used operations (managing databases, tables, columns, relations, indexes, users, permissions, etc) 
can be performed via the user interface, while you still have the ability to directly 
execute any SQL statement - see http://www.phpmyadmin.net/

## Requirements and known issues

Version 5.x of the TYPO3 phpMyAdmin extension includes the latest release of phpMyAdmin (4.x).
phpMyAdmin 4.4.x is officially supported for security fixes only until October 1, 2016!

If you're in need of an older version compatible with PHP 5.2 and MySQL 5 just use one of the 4.x 
releases. The 4x releases were supported for security fixes only until Jan 1, 2016.

## Installation

From 5.2 on you need to use composer to install. Additionally a post-install command in your TYPO3 root composer.json file
has to be defined as composer does not support run scripts of dependecies.

In this post-install-cmd script run: composer run-script post-install-cmd -d typo3conf/ext/phpmyadmin

### Update

Remove complete extension folder and install extension again (to execute post-install-cmd).