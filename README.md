# magento_iis_setup
### Setup for magento on IIS

http://www.drupalonwindows.com/en/blog/installing-magento-windows-and-iis#tooling

Volg bovenstaande tutorial om Magento correct op te zetten.
###### installeren van volgende tools:
- Chocolatey
- IIS chef
- php via choco
- php.ini ook aanpassen met vermelde lijnen.

Het downloaden van magento en de patch uitvoeren mag je skippen. Het git gedeelte uiteraard ook.

Database vullen met basic_setup.sql

Na installeren van de tools kan je rechtstreeks doorgaan naar het deployen van de applicatie.
Het deployen doet alles zelf waardoor je zelf niets in IIS moet toevoegen/aanpassen

De setup dien je normaal gezien niet meer uit te voeren. De applicatie zou moeten werken. 

Indien je geen stijl moest hebben aan de admin kant, voer dan even volgend command uit:

`php bin/magento setup:static-content:deploy -f`

Dit kan je best doen vanuit de aangemaakte folder na het deployen. 
Dit is normaal gezien {schijf}:\chef\_apps\chf_magento_xxxx\runtime\php


