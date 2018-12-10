# OpenCart-Whoops
Pretty print errors module for OpenCart, powered by the [Filp/Whoops](https://github.com/filp/whoops) package. For an example of these pretty print errors, see the [example](http://filp.github.io/whoops/demo/) created by the developers of Filp/Whoops. 

## Installation
This module comes with the source files for the Whoops library already downloaded, so there is no need to run composer install. Just zip up the files within '/module' and make sure the zipped file is renamed to have '.ocmod.zip' as the extenstion. For example: 'modulename.ocmod.zip'.

Install within OpenCart, as you would with any other module, and it should work straight out of the box. If you need to test it to double check, just cause a syntax error or throw a random exception to see if the module picks it up.

If for any reason you decide you'd like to disable this extension it can be done one of two ways. Just like all modules, it can be disbaled within the administration panel at any time. This will disable the module across the entire site. However if you want to disable it just on the frontend, or just within the admin panel, then you'll need to add the following to the config file:

For disabling in the admin panel, add to './admin/config.php'. For the frontend, add to './config.php'.

```PHP
define(OC_DEBUG, FALSE);
```