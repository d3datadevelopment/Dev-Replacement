[![deutsche Version](https://logos.oxidmodule.com/de2_xs.svg)](README.de.md)
[![english version](https://logos.oxidmodule.com/en2_xs.svg)](README.md)

# dauerhaftes Entfernen der Entwicklerpakete, wenn diese nicht benötigt werden

Dieses Paket entfernt die ungenutzten OXID Entwicklerpakete aus der Shopinstallation und verhindert damit mögliche Konflikte bei späteren Updates oder Installationen.

Auch wenn die --no-dev/--update-no-dev-Parameter vergessen werden, werden keine Entwicklerpakete installiert.

## Installation

wenn die Entwicklerwerkzeuge nicht benötigt werden und von der Installation entfernt werden sollen

* Starte die Befehle in der Konsole Deines Shopprojektes. Passe die Anweisungen an, wenn Deine Installation dies erfordert.

    ```
    composer require d3/oxid-dev-replacement --no-scripts --no-plugins
    composer remove phpunit/phpcov pdepend/pdepend behat/mink-goutte-driver oxid-esales/mink-selenium-driver squizlabs/php_codesniffer mikey179/vfsstream
    ```

## Deinstallation

wenn die Entwicklerwerkzeuge wieder benötigt werden

* Starte die Befehle in der Konsole Deines Shopprojektes. Passe die Anweisungen an, wenn Deine Installation dies erfordert.

    `composer remove d3/oxid-dev-replacement`
