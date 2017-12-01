# WillMill

This is the WillMill project based on [Phalcon Framework](https://github.com/phalcon/cphalcon).

Please write us if you have any feedback.

Thanks.

## NOTE

The master branch will always contain the latest stable version.
If you wish to check older versions or newer ones currently under development, please switch to the relevant branch.

## Get Started

### Requirements

To run this application on your machine, you need at least:

* >= PHP 5.5
* >= Phalcon 3.2
* Apache Web Server with `mod_rewrite enabled`, and `AllowOverride Options` (or `All`) in your `httpd.conf` or Nginx Web Server
* Latest [Phalcon Framework](https://github.com/phalcon/cphalcon) extension installed/enabled
* MariaDB >= 10.2 (or may work on MySQL >= 5.5)

Then you'll need to create the database and initialize schema:

```bash
echo 'CREATE DATABASE willmill' | mysql -u root
cat schemas/willmill.sql | mysql -u root willmill
```

Next, create user `willmill` with all privileges for DB `willmill`.

Also you must override application config by creating `app/config/config.dev.php` (already gitignored)
and typing there real password for `willmill` user for DB connection.

### Installing Dependencies via Composer

WillMill's dependencies must be installed using Composer. Install composer in a common location or in your project:

```bash
curl -s http://getcomposer.org/installer | php
```

Run the composer installer:

```bash
cd willmill
php composer.phar install
```

**NOTE** After the installation, please ensure that the following folders have write permissions set:
- `cache`

## Improving this Sample

Phalcon is an open source project and a volunteer effort.

## License

WillMill is proprietary software, (c) all right reserved.
