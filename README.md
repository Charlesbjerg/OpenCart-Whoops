# OpenCart-Whoops
Pretty print errors module for OpenCart, powered by the [Filp/Whoops](https://github.com/filp/whoops) package.

## Installation
This module comes with the source files for the Whoops library already downloaded, so there is no need to run composer install. Just zip up the files within '/module' and make sure the zipped file is renamed to have '.ocmod.zip' as the extenstion. For example: 'modulename.ocmod.zip'.

Install within OpenCart, as you would with any other module, and it should work straight out of the box. If you need to test it to double check, just cause a syntax error or throw a random exception to see if the module picks it up.
