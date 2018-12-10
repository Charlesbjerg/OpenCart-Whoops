# OpenCart-Whoops
Pretty print errors module for OpenCart, powered by the [Filp/Whoops](https://github.com/filp/whoops) package. For an example of these pretty print errors, see the [example](http://filp.github.io/whoops/demo/) created by the developers of Filp/Whoops. 

## Installation
This module comes with the source files for the Whoops library already downloaded, so there is no need to run composer install. Just zip up the files within '/module' and make sure the zipped file is renamed to have '.ocmod.zip' as the extenstion. For example: 'modulename.ocmod.zip'.

Install within OpenCart, as you would with any other module. Then add the code below to the two config files, './config.php' and './admin/config.php'.

```PHP
// DEBUG 
define('OC_DEBUG', true);
```

The module will continue to output a PHP warning for an undefined constant if the above is not added. If you also need to test that the module is running just to double check, just cause a syntax error or throw a random exception to see if the module picks it up.

If for any reason you decide you'd like to disable this extension, it can be done one of two ways. Just like all modules, it can be disbaled within the administration panel at any time. This will disable the module across the entire site. However if you want to disable the module on just the frontend or just the admin panel, then change the 'OC_DEBUG' constant to false in the corresponding config file.

