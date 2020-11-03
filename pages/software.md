# (Open Source) Software
welke softwarepakketten gebruikt Commons Lab en voor welke processen. 

Op dit moment maakt Commons Lab Antwerpen (nog) geen gebruik van open source software maar neemt ze diensten af bij leveranciers: 
- mailserver bij Spinternet (roundcube php pakket)
- bestanden delen met GSuite
- CMS website bij Squarespace
- aanzet to CRM bij Hubspot
- zelfgebouwde excels voor de administratie en tijdregistratie

In de organisatie zijn personen actief met ervaring met en allertheid voor eerlijke (open source) software. Momenteel worden deze voorstellen gesignaleerd in het slack kanaal van Commons lab, bediscussieerd maar er is geen structurele manier om met deze voorstellen om te gaan. 

## Mailserver en filesharing
Zelf een mailserver met open source software opzetten en laten draaien vraagt heel wat onderhoud (en bijhorende kosten) om hetzelfde aanbod te bekomen als Google of Microsoft aanbieden. Zeker wanneer je ook kijkt naar de aan het systeem gekoppelde filesharing systeem van 1 TB. Ik denk dat we die middelen, energie en tijd beter steken in het uitwerken van goede open source pakketten voor kerntaken van de organisatie in tegenstelling tot de ondersteunende mail en filesharing.

'''
Er werd gekozen om dit aspect uit te rollen met office365. 
'''

## Website
Services als Squarespace, Wix hebben het voordeel dat ze eenvoudig 'drag en drop' een website laten bouwen. Je hoeft je niet bezig te houden met het updaten van plugins, hosting, ... Daartegenover staat wel dat deze meer gesloten systemen weinig ruimte laten tot het delen van data, custom design, ...

Uit de [analyse van de huidige toestand](pages/analyse.md#communicatie) blijkt dat er nog geen duidelijk plan is wat nu juist de website moet zijn en hoe de communicatiestrategie naar buiten moet zijn. Een herwerken van de website naar een open source pakket is nog niet aan de orde. Vooralleer een (hernieuwde) website wordt ontwikkeld moet er een duidelijk antwoord zijn op de vragen: 
- welke rol speelt de website in onze organisatie: moet de website tools bevatten of niet
- investeren we in content creatie of niet: wat voor type website maken we
- welke rol speelt de website in het commons ecosysteem in vlaanderen: heeft de website een hub rol of niet

Indien de website herbouwd wordt zou het voorstel zou zijn om **bij het bouwen van websites over te stappen op het open source technologie van Wordpress** ([wordpress.org](https://wordpress.org/about/license/)) dat een heel grote community kent van developpers die continu verder bouwen aan dit pakket en de afgeleide open source plugins. Indien er grote noodzaak is bestaat er ook een markt aan bedrijven die betalende plugins en thema's voorziet. 

Bijkomend voordeel van Wordpress als backbone voor de CRM in vergelijking met python of javascript frameworks (Django, React, Vue.js, Angular) is dat Wordpress draait op een eenvoudige web server setup (MySQL - en .php files). Een webhosting die een degelijke php hosting aanbiedt (minstens Php 7.2) is betaalbaar te vinden. De hosting voor de javascript frameworks is complexer en komt vaak duurder uit. 

Drupal, het andere sterke php based framework, zet ook sterk in op haar open source karakter. Wordpress heeft als grootste voordeel ten opzichte van Drupal dat Wordpress een veel grotere community heeft en het daardoor eenvoudiger is om specifieke plugins te vinden die tegemoet komen aan de noden. Daarnaast is de leercurve van Drupal stijler. Drupal heeft dan weer als voordeel dat de kern van het CMS sterker is en de basisbeveiliging beter is uitgewerkt. **Een keuze voor Wordpress betekent dus ook dat er bijkomende aandacht moet besteedt worden aan beveiliging.**

In het Wordpress pakket zit ook een [REST API](https://developer.wordpress.org/rest-api/) ingebouwd. Het is dus mogelijk om de data van Commons Lab via een API te ontsluiten. Bij het ontwerp van elke website dient dus ook de afweging gemaakt te worden: welke tabellen/Data en in welke vorm willen we uit deze website ontsluiten zodat andere organisaties en individuën hiermee aan de slag kunnen gaan.

### Webshops 
Momenteel worden samenaankopen georganisseerd met google forms en manuele controles op lijsten. De vraag komt naar boven of we niet kunnen experimenteren met webshops om dit proces te vergemakkelijken. Hierbij zijn volgende opties: 
- woocommerce (wordt gebruikt door de theatergarage)
- shopify (geen open source)

### Leerplatformen
Er zijn geen gestructureerde leerplatformen in gebruik. Mogelijke pistes zijn om te experimenteren met volgende open source alternatieven: 
- moodle (wordt gebruikt door bv. syntra)
- learnpress (wordt gebruikt door het Bisdom Antwerpen)

**TODO**:
- afwegingskader en flow toevoegen

## CRM
Nog uit te werken: Hubspot vs Espo CRM (php based CRM)
- spelen met Espo CRM kan eenvoudig via Cloudron: [link](https://cloudron.io/store/com.espocrm.cloudronapp.html)
