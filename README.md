# Activisme_BE - PHP-CS-FIXER rules 

Our PHP-CS-FIXER rules that we use troughout our projects. 

## Install 

This package is custom built for Activisme_BE projects and is therefore not registered  on packagist. 
In order to install it via composer you must specify this extra repository in `composer.json`: 

```json
"repositories": [{
  "type": "vcs", 
  "url": "https://github.com/activisme-be/php-cs-fixer-rules"
}]
```

You can install the package via composer: 

```bash
$ composer require activisme-be/php-cs-fixer-rules --dev
```

## Overview 

This package provides the base styleguide rules for php-cs-fixer in our Laravel applications. 

## Example 

```php 
<?php

// filename: .php_cs.dist

$finder = PhpCsFixer\Finder::create()
  ->in([
    __DIR__.'/app',
    __DIR__.'/config',
    __DIR__.'/database',
    __DIR__.'/routes',
    __DIR__.'/tests',
  ]);

return ActivismeBE\PhpCsRules($finder);
```

## Changelog 

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## License 

The MIT license (MIT). Please see [License file](LICENSE.md) for more information.
