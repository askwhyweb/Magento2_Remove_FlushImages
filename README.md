# Mage2 Module OrviSoft Cache

    `orvisoft/module-cache`

 - [Main Functionalities](#main-functionalities)
 - [Installation](#installation)


## Main Functionalities
This module removes ability to "Flush Catalog Images Cache" and "Pregenerated product images files". In some production instances where default mode of Magento is used, its essential to disallow ability to flush catalog images and pre-generated product images.

## Installation
\* = in production please use the `--keep-generated` option

### Type 1: Zip file

 - Unzip the zip file in `app/code/OrviSoft`
 - Enable the module by running `php bin/magento module:enable OrviSoft_Cache`
 - Apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`

### Type 2: Composer

 - Make the module available in a composer repository for example:
    - private repository `repo.magento.com`
    - public repository `packagist.org`
    - public github repository as vcs
 - Add the composer repository to the configuration by running `composer config repositories.repo.magento.com composer https://repo.magento.com/`
 - Install the module composer by running `composer require orvisoft/module-cache`
 - enable the module by running `php bin/magento module:enable OrviSoft_Cache`
 - apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`
