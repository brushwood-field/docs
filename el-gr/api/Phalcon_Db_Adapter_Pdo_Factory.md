---
layout: default
language: 'el-gr'
version: '4.0'
title: 'Phalcon\Db\Adapter\Pdo\Factory'
---
# Class **Phalcon\Db\Adapter\Pdo\Factory**

*extends* abstract class [Phalcon\Factory](Phalcon_Factory)

*implements* [Phalcon\FactoryInterface](Phalcon_FactoryInterface)

[Source on GitHub](https://github.com/phalcon/cphalcon/tree/v{{ page.version }}.0/phalcon/db/adapter/pdo/factory.zep)

Loads PDO Adapter class using 'adapter' option

```php
<?php

use Phalcon\Db\Adapter\Pdo\Factory;

$options = [
    "host"     => "localhost",
    "dbname"   => "blog",
    "port"     => 3306,
    "username" => "sigma",
    "password" => "secret",
    "adapter"  => "mysql",
];
$db = Factory::load($options);

```

## Methods

public static **load** ([Phalcon\Config](Phalcon_Config) | *array* $config)

protected static **loadClass** (*mixed* $namespace, *mixed* $config) inherited from [Phalcon\Factory](Phalcon_Factory)

...