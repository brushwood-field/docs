---
layout: default
language: 'es-es'
version: '4.0'
title: 'Phalcon\Paginator\Factory'
---
# Class **Phalcon\Paginator\Factory**

*extends* abstract class [Phalcon\Factory](Phalcon_Factory)

*implements* [Phalcon\FactoryInterface](Phalcon_FactoryInterface)

[Código fuente en GitHub](https://github.com/phalcon/cphalcon/tree/v{{ page.version }}.0/phalcon/paginator/factory.zep)

Carga un adaptador de Paginator utilizando la opción 'adapter'

```php
<?php

use Phalcon\Paginator\Factory;

/**
 * The `modelsManager` is automatically created when you instantiate your DI
 * container using the `FactoryDefault` class. It returns a 
 * [Phalcon\Mvc\Model\Manager](Phalcon_Mvc_Model_Manager) object
 */

$builder = $this->modelsManager->createBuilder()
                ->columns("id, name")
                ->from("Robots")
                ->orderBy("name");

$options = [
    "builder" => $builder,
    "limit"   => 20,
    "page"    => 1,
    "adapter" => "queryBuilder",
];
$paginator = Factory::load($options);

```

## Métodos

public static **load** ([Phalcon\Config](Phalcon_Config) | *array* $config)

protected static **loadClass** (*mixed* $namespace, *mixed* $config) inherited from [Phalcon\Factory](Phalcon_Factory)

...