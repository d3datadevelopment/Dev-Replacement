[![deutsche Version](https://logos.oxidmodule.com/de2_xs.svg)](README.de.md)
[![english version](https://logos.oxidmodule.com/en2_xs.svg)](README.md)

# permanently removing the developer package when they aren't needed

This package removes the unused OXID development package from the shop and prevents conflicts in later updates or installations.

Even if the --no-dev/--update-no-dev parameters are forgotten, no developer packages will be installed.

## Install

if the development tools are not used and should be removed from the shop installation

* Run these composer commands in the console of your shop project. Adjust this instruction if your installation requires it.

    ```
    composer require d3/oxid-dev-replacement --no-scripts --no-plugins
    composer remove phpunit/phpcov pdepend/pdepend behat/mink-goutte-driver oxid-esales/mink-selenium-driver squizlabs/php_codesniffer mikey179/vfsstream
    ```

    
## Uninstall

if the dev tools are to be used again

* Run this composer command in the console of your shop project. Adjust this instruction if your installation requires it.

    `composer remove d3/oxid-dev-replacement`
