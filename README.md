# Development package replacement if dev tools are not used

This package removes the unused OXID development package from the shop and prevents conflicts in later updates.

Also, if the --no-dev/--update-no-dev parameter is forgotten, not all developer packages will be installed.

## Install

if the development tools are not used and should be removed from the shop installation

* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer require d3/oxid-dev-replacement --update-no-dev`
    
## Uninstall

if the dev tools are to be used again

* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer remove d3/oxid-dev-replacement --update-no-dev`
