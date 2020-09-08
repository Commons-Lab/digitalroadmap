# (Open Source) Software
welke softwarepakketten gebruikt Commons Lab en voor welke processen. 

Op dit moment maakt Commons Lab Antwerpen (nog) geen gebruik van open source software maar neemt ze diensten af bij leveranciers: 
- mailserver bij Spinternet (roundcube php pakket)
- bestanden delen met GSuite
- CMS website bij Squarespace
- aanzet to CRM bij Hubspot

## Mailserver en filesharing
Zelf een mailserver met open source software opzetten en laten draaien vraagt heel wat onderhoud (en bijhorende kosten) om hetzelfde aanbod te bekomen als Google of Microsoft aanbieden. Zeker wanneer je ook kijkt naar de aan het systeem gekoppelde filesharing systeem van 1 TB. Ik denk dat we die middelen, energie en tijd beter steken in het uitwerken van goede open source pakketten voor kerntaken van de organisatie in tegenstelling tot de ondersteunende mail en filesharing.

## Website
Services als Squarespace, Wix hebben het voordeel dat ze eenvoudig 'drag en drop' een website laten bouwen. Je hoeft je niet bezig te houden met het updaten van plugins, hosting, ... Daartegenover staat wel dat deze meer gesloten systemen weinig ruimte laten tot het delen van data, custom design, ...

Het voorstel zou zijn om **bij het bouwen van websites over te stappen op het open source pakket van Wordpress** ([wordpress.org](https://wordpress.org/about/license/)) dat een heel grote community kent van developpers die continu verder bouwen aan dit pakket en de afgeleide open source plugins. Indien er grote noodzaak is bestaat er ook een markt aan bedrijven die betalende plugins en thema's voorziet. 

Bijkomend voordeel van Wordpress als backbone voor de CRM in vergelijking met python of javascript frameworks (Django, React, Vue.js, Angular) is dat Wordpress draait op een eenvoudige web server setup (MySQL - en .php files). Een webhosting die een degelijke php hosting aanbiedt (minstens Php 7.2) is betaalbaar te vinden. De hosting voor de javascript frameworks is complexer en komt vaak duurder uit. 

Drupal, het andere sterke php based framework, zet ook sterk in op haar open source karakter. Wordpress heeft als grootste voordeel ten opzichte van Drupal dat Wordpress een veel grotere community heeft en het daardoor eenvoudiger is om specifieke plugins te vinden die tegemoet komen aan de noden. Daarnaast is de leercurve van Drupal stijler. Drupal heeft dan weer als voordeel dat de kern van het CMS sterker is en de basisbeveiliging beter is uitgewerkt. **Een keuze voor Wordpress betekent dus ook dat er bijkomende aandacht moet besteedt worden aan beveiliging.**

### Webshops 
Wordpress + Woocommerce vs. Shopify vs. ....

### Leerplatformen
Wordpress + Learnpress vs ...

### Open data
In het Wordpress pakket zit ook een [REST API](https://developer.wordpress.org/rest-api/) ingebouwd. Het is dus mogelijk om de data van Commons Lab via een API te ontsluiten. Bij het ontwerp van elke website dient dus ook de afweging gemaakt te worden: welke tabellen/Data en in welke vorm willen we uit deze website ontsluiten zodat andere organisaties en individuën hiermee aan de slag kunnen gaan.

**TODO**:
- afwegingskader en flow toevoegen
- basistemplate in git voorzien zodat een API pagina aan een website kan worden toegevoegd.

## CRM
Nog uit te werken: Hubspot vs Espo CRM (php based CRM)
- spelen met Espo CRM kan eenvoudig via Cloudron: [link](https://cloudron.io/store/com.espocrm.cloudronapp.html)
