Leaflet Bundle for Symfony2

## Current Version

Leaflet v0.7.0

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "bmatzner/leaflet-bundle": "~0.7"
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
        new Bmatzner\LeafletBundle\BmatznerLeafletBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/leaflet-bundle
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

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<link rel="stylesheet" href="{{ asset('bundles/bmatznerleaflet/css/leaflet.css') }}" />
<!--[if lte IE 8]>
    <link rel="stylesheet" href="{{ asset('bundles/bmatznerleaflet/css/leaflet.ie.css') }} />
<![endif]-->
<script type="text/javascript" src="{{ asset('bundles/bmatznerleaflet/js/leaflet.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://leafletjs.com/
2. http://symfony.com/
