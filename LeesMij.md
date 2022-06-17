## WETTELIJKE WAARSCHUWING
#### !!! HET GEBRUIK VAN DEZE APPLICATIE IS GEHEEL OP EIGEN RISICO
#### !!! Ik accepteer geen enkele verantwoordelijkheid.
#### !!! Het opheffen van de snelheidslimiet maakt de fiets illegaal voor gebruik op de openbare weg in de meeste landen, in ieder geval in de Europeese-unie.
#### !!! Mogelijk vervalt de garantie op de fiets

# Cowboy Untamed
Een **Android app om de snelheidslimiet op te heffen** van de Cowboy V1+, V2, V3 or V4(ST), maakt de fiets sneller en nog een paar andere leuke *tweaks* om de fiets nog leuker te maken.<br><br>

## Download
[Versie overzicht](https://github.com/Imaginous/Cowboy_Untamed/releases)<br>
Klik op de link naar het betreffende *.APK* bestand onder *Assets*.

## Doneren
Mocht je mijn werk waarderen dan is een kleine donatie altijd welkom.
[Klik hier](https://github.com/Imaginous/Cowboy_Untamed/edit/main/README.md#donate) om te doneren via PayPal of iDeal.

## Korting op een nieuwe Cowboy V3, V4(ST) fiets
Mocht je een nieuwe Cowboy fiets willen kopen, dan kan je via [deze link](https://share.cowboy.com/r/michelv3) €100 korting krijgen op jouw nieuwe fiets.<br>
Bij genoeg verwijzingen krijg ik een attentie van Cowboy. 

## Introductie
Ik leg hier beknopt in het Nederlands uit hoe je Untamed kan gebruiken.
Voor de uitgebreide informatie verwijs ik graag naar het [Engelse deel](https://github.com/Imaginous/Cowboy_Untamed#readme).

*Eigenschappen:*
- Snelheidslimiet verwijderen van de Cowboy.
- *Field weakening* instellen om de maximum snelheid te verhogen (tot 35-38km/u).
- [*Dashboard* om het ondersteuningsniveau in te stellen tijdens het fietsen.](https://github.com/Imaginous/Cowboy_Untamed/edit/main/README.md#dashboard)
- Inschakelen van *Auto Unlock* voor het V1+ model.
- Snelkoppelingen om de fiets in/uit te schakelen. Deze kan je bijvoorbeeld gebruiken met *Tasker*.
- *1 keer instellen en klaar*. Als je alleen de snelheidslimiet er af wilt halen en eventueel de snelheid wilt verhogen kan je dit 1 keer instellen en daarna heb je de app alleen voor wijzigingen nodig.<br>
- Je kan dus even een Android toestel lenen en daarna gewoon weer jouw iPhone gebruiken.
- [*Quick Launch Presets*](https://github.com/Imaginous/Cowboy_Untamed/blob/8d6e54f92d7533ade69096deab1b06cd6be3ff6f/Presets.md)


<p float="left">
<img src="https://user-images.githubusercontent.com/68418842/119372390-8cab3680-bcb7-11eb-8d2c-c685640cb8ac.png" alt="Screenshot main app" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/119372491-a9e00500-bcb7-11eb-87df-e4dcc1d19b9b.png" alt="Screenshot expert page" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/121254562-b1ec9700-c8aa-11eb-9aaa-fff43845ab1b.png" alt="Screenshot quick launch presets" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/119372515-b2384000-bcb7-11eb-9b1a-633b93c2d93e.png" alt="Screenshot shortcuts main app" width="250"/>
<img src="https://user-images.githubusercontent.com/68418842/121254592-badd6880-c8aa-11eb-86db-a6b5ab1bea7f.png" alt="Screenshot shortcuts presets app" width="250"/>
</p>

Dit is puur een hobby project. Ik ben gek op elektronica en programmeren en was overtuigd dat er meer uit deze mooie Cowboy fietsen te halen moest zijn.

Speciale dank gaat naar *Runereader* voor het opensource maken van de *Bronco* app. Gezien dit mijn eerste Android app is heb ik veel geleerd over het maken van apps door zijn app.
Ik heb veel informatie opgevraagd bij de fabrikant (ASI) van de motorcontroller van de fiets. Ik heb de gegevens gekregen, maar moest wel een *Non Disclosure Agreement* tekenen. Hierdoor kan ik de code niet openbaar maken.

Zoals gezegd is het puur hobby, de software is zoals hij is.

## Installatie
Op de Android telefoon moet er toestemming worden gegeven om software te installeren vanuit *onbekende bronnen (Unknown Sources)*. Daarna zou je het *.APK* bestand mogen installeren.<br>
Gezien de aard van de software is het moeilijk om hem toegelaten te krijgen tot de *Play-Store*.

- Ga naar het *Instellingen* menu op jouw Android telefoon.
- Ga naar *beveiliging*.
- Vink de optie *Onbekende Bronnen* aan.

Als het goed is kan je nu het *APK* bestand downloaden en installeren.<br><br>
Om de veiligheid van de telefoon te garanderen en dat je niet per abuis zomaar software uit andere bronnen kunt installeren raad ik aan om de *Onbekende Bronnen* weer uit te schakelen na het installeren van Untamed.<br><br>
**Let op:** Sommigen kopen een oude Android telefoon voor deze app, zorg ervoor dat je minimaal Android versie **7.1.1 of hoger** hebt.

## Gebruik / uitleg
Je kan met deze app dus de snelheidslimiet van jouw Cowboy V1/2/3/4(ST) halen.<br>
Echter zal je met  alleen het verwijderen van de limiet nog steeds niet veel sneller dan 28-30km/u kunnen fietsen, hiervoor komt *field weakening* om de hoek kijken. Zodra de motor boven het maximale aandrijftoerental komt, gaat deze als een soort dynamo werken en werkt verdere versnelling tegen. Dit komt puur door het magnetischeveld wat wordt opgewekt.<br>
Nu heeft de motorcontroller een functie om dit op te heffen: *field weakening*. Door een tegengestelde stroom door de spoelen te sturen wordt het tegenwerken (deels) opgeheven. Dit heeft een nadeel... het kost extra energie, dus gaat de batterij sneller leeg.

Ik raad een *field weakening* waarde aan van:
- 18 voor een C1+ en C2
- 15 voor een C3 en C4
- 13 voor een C4ST

Het verschil in waarden heeft te maken met de verschillende verzetten (overbrengingsverhouding) van de diverse Cowboy modellen. Het probleem is bij de nieuwere modellen dat het met een kleiner verzet echt snel trappen wordt bij hogere snelheden.
De maximum aanbevolen waarde is 20%. De uiterste limiet is 25% aldus fabrikant ASI, echter met de opmerking dat dit bij zware/langdurige belasting schade kan opleveren. **Dus ga gewoon niet hoger dan 20%**.<br>
Daarnaast... hoe hoger de waarde hoe meer batterij je verbruikt.

Zorg dat de fiets is gekoppeld met jouw Android toestel en wordt getoond onder de bluetooth apparaten.
Ik adviseer eigenlijk om eerst de fiets te koppelen met de originele Cowboy app. Dan vervolgens onder de instellingen van de fiets de *Paring Code* op te schrijven.
Vervolgens gooi je de fiets weg bij de bluetooth instellingen (als deze er staat) en zoek je naar nieuwe bluetooth apparaten. Voeg vervolgens de *Cowboy* opnieuw toe en gebruik de opgeschreven koppelcode. Eventueel kan je de naam nog aanpassen mocht je meerdere Cowboy fietsen gaan koppelen.

- **Sluit de originele Cowboy app volledig af.**
- Zorg ervoor dat er geen andere telefoons of apparaten zijn verbonden met de fiets.
- Ga vlak bij de fiets staan.
- Open de Cowboy Untamed app.
- Selecteer de juiste Cowboy fiets (eventueel kan je bij het koppelen de bluetooth naam van de fiets aanpassen). 
- Zet het *connect* schuifje in de *aan* stand.
- Wacht rustig totdat de app verbinding heeft gemaakt.
- De meeste opties worden pas actief als de verbinding tot stand is gekomen. De huidige waarden worden getoond na het verbinden.
- Selecteer *Torque (no speed limit)* - Als je de snelheidslimiet wilt opheffen.
- Vul de gewenste waarde in voor *field weakening*, zeg 15.
- Druk op de **TEST** knop. (De instellingen worden naar de fiets gestuurd, maar nog niet definitief vast gelegd. Wordt de fiets nu uitgeschakeld dan zijn de instellingen weer weg).
- Om de waarden "definitief" vast te leggen klik je op de **FLASH** knop. De waarden worden nu vastgelegd in de motorcontroller.
- Zet het *connect* schuifje in de *uit* stand. De fiets word nu uitgeschakeld.
- Je kan nu weer de originele Cowboy app gebruiken.

#### Snelheidslimiet herstellen
Als je niet zelf met *Expert Settings* aan het spelen bent geweest kan je onderstaande methode gebruiken om de originele waarden weer te herstellen.
- Zet het *connect* schuifje in de *aan* stand.
- Druk op de **DEFAULTS** knop.
- Om de waarden "definitief" vast te leggen klik je op de **FLASH** knop. De waarden worden nu vastgelegd in de motorcontroller.
- Zet het *connect* schuifje in de *uit* stand. De fiets word nu uitgeschakeld.

#### Overige functies van de app
Uiteraard is er nog veel meer mogelijk met de app. Hiervoor verwijs ik even door naar de [Engelse documentatie](https://github.com/Imaginous/Cowboy_Untamed#readme).

## FAQ

- **Is this information available in English?**<br>**Yes**, [just click here](https://github.com/Imaginous/Cowboy_Untamed#readme).
- **Komt er een IOS versie?**<br>**Nee**, helaas heb ik geen Apple developers account (en ben ook niet van plan er een te nemen).<br>Maar je kan de aanpassing ook **handmatig** doen: [IOS.md](https://github.com/Imaginous/Cowboy_Untamed/blob/main/IOS.md).
- Kan ik een andere Android telefoon gebruiken/lenen om de instellingen aan te passen?<br>Ja, dit kan voor de snelheidslimiet *hack*. Je kan hierna dus ook weer gewoon jou iPhone gbruiken. Voor het *presets* en/of het *Dashboard* heb je uiteraard actief een Android telefoon nodig.
- Als ik het *APK* bestand download gebeurt er niets?<br>Het bestand is op de achtergrond gedownload. Ga naar het menu rechts boven in *Chrome* en selecteer *Downloads*. Kies nu het *APK* bestand en installeer het.<br>Je kan natuurlijk ook gebruikmaken van een bestandsmanager zoals *CX File Explorer*, ga naar Downloads en installeer de APK.
- Kan alles ongdeaan worden gemaakt?<br>Ja, als er geen geen gebruik is gemaakt van *Expert Functions* en je start Untamed even schoon op en zorgt dat de fiets wordt ingeschakeld met Untamed dan kan je op de **DEFSAULTS** knop gevolgd door de **FLASH** knop drukken om de snelheidslimiet weer te activeren. .
- I wil een donatie doen, hoe?<br>[Klik hier](https://github.com/Imaginous/Cowboy_Untamed/blob/main/README.md#donate) voor een donatie via PayPal of iDeal.
