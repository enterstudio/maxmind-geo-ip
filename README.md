maxmind-geo-ip-bundle
=====================
A symfony bundle for geo location with the maxmind geo database.

Installation
----------- 
You can install this library with composer or include it manually in your project.

Quick start
-----------

Set the path to the maxmind database in your config yml.
```php
gtuk_geo_ip:
    db_path: "../GeoLite2-City.mmdb"
```

After this you can call the service and execute different methods.

```php
$geoIp = $this->get('gtuk_geo_ip');

$cityRecord = $geoIp->city('97.77.104.22'));
```

##Available methods

For all available methods take a look at https://github.com/maxmind/GeoIP2-php

##TODOS

- Add Tests
- Symfony db install command
- Add maxmind web api service