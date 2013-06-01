ayah-module
===========

A ZF2 module for Are You A Human's PlayThru captcha alternative.

# INSTALLATION

Add the following to your composer.json file:
```
"repositories": [
    {
        "type": "vcs",
        "url": "https://github.com/austinsmorris/ayah-module.git"
    }
],
"require": {"austinsmorris/ayah-module": "dev-master"}
```

Navigate to `/vendor/austinsmorris/ayah-module/src/AYAH/PlayThru`.  Rename the file
`ayah_config.php.dist` to `ayah_config.php`.  Open this file and enter your publisher
and scoring keys as indicated.

## SYSTEM REQUIREMENTS
-------------------

austinsmorris/ayah-module requires PHP 5.3.3 or later.

## GETTING STARTED

ayah-module registers a controller plugin and view helper named 'ayah' to simplify the
use of the PlayThru library.

In a controller:
```php
$this->ayah()
```
This will return the score result to determine if the submitted form came from a human.

In a view script:
```php
<?php echo $this->ayah(); ?>
```
This will render the PlayThru plugin.

For a working example, see:
https://github.com/austinsmorris/ayah-module-demo

## VERSION

This version of ayah-module uses the AYAH php bundle version 1.1.7.
