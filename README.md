# CKEditor Office 2013 Skin Bundle for Symfony2
Symfony2 Bundle to integrate the CKEditor skin Office 2013

## Current Version

Quick Table v1.0.4

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-office2013-skin-bundle": "~1.0.6"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\CKEditorOffice2013SkinBundle\StingerCKEditorOffice2013SkinBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-office2013-skin-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

``` yaml
trsteel_ckeditor:
    skin: 'office2013,../../bundles/stingerckeditoroffice2013skin/'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/office2013
2. http://symfony.com
