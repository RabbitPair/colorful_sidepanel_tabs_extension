# Changelog

Alle belangrijke wijzigingen in dit project worden in dit bestand gedocumenteerd.

Dit project houdt zich aan [Semantische Versiebeheer](https://semver.org/).

----

## [Niet uitgebracht]

- **Geplande Momentopnamen**: Automatisch momentopnamen opslaan op gespecificeerde intervallen. Deze functie zorgt ervoor dat uw werk periodiek wordt geback-upt, waardoor een vangnet tegen gegevensverlies wordt geboden.

----
## [2.11.0] - 2024-10-07
### Toegevoegd
- **Tabbladmenu**: Nieuwe menu's zijn toegevoegd:
  - **Tabbladtitel hernoemen**: Hiermee kunt u de tabbladtitel wijzigen. Standaard is de optie om de URL-instellingen te onthouden geselecteerd, zodat de titel automatisch wordt bijgewerkt de volgende keer dat u de URL opent.
  - **Tabblad verplaatsen naar nieuw venster**: Hiermee kunt u het tabblad naar een nieuw venster verplaatsen.
  - **Tabblad verplaatsen naar een ander venster**: Hiermee kunt u het tabblad naar een ander bestaand venster verplaatsen.
  - **Tabblad uit groep verwijderen**: Hiermee kunt u het tabblad uit de huidige groep verwijderen.

- **Tabbladinstellingen**: Nieuwe opties zijn toegevoegd aan de tabbladinstellingen:
  - **Maximaal aantal weergegeven regels voor tabbladtitel**: Stel het maximale aantal regels in dat wordt weergegeven voor tabbladtitels. Extra regels worden verborgen.
  - **Maximaal aantal weergegeven regels voor groepstitel**: Stel het maximale aantal regels in dat wordt weergegeven voor groepstitels. Extra regels worden verborgen.
  - **Breedte van ingeklapte groepstitel**: Stel de breedte van de groepstitel in wanneer de groep is ingeklapt.
  - **Aantal tabbladen in groep weergeven**: Toont het aantal tabbladen in elke groep naast de groepsnaam.

- **Site-instellingen**: Nieuwe opties zijn toegevoegd aan de site-instellingen:
  * **Pagina actief houden**: Wanneer ingeschakeld, mag het tabblad door de browser worden verwijderd. Als u prestatie-instellingen inschakelt en een tijd instelt om inactieve tabbladen te verwijderen, wordt het tabblad na de opgegeven tijd verwijderd. Als dit is uitgeschakeld, wordt het tabblad niet verwijderd.
  * **Automatisch lid worden van groep**: Wanneer ingeschakeld, maakt de site automatisch een groep aan of wordt lid van de opgegeven groep.
  * **Incognitomodus**: Wanneer ingeschakeld, kunt u ervoor kiezen om automatisch browsegegevens te wissen bij het bezoeken van de site. Dit omvat verschillende configureerbare opties: Cookies, Geschiedenis, CacheStorage, Bestanden, IndexedDB, Lokale opslag, ServiceWorkers en WebSQL. Houd er rekening mee dat de toestemming voor browsingData niet wordt gebruikt om te voorkomen dat er extra machtigingen worden aangevraagd.
  * **Automatisch vernieuwen**: In de linkconfiguratie-instellingen kunt u URL's opgeven die automatisch worden vernieuwd, met ondersteuning voor reguliere expressies.

### Gewijzigd
- **Geavanceerde Picture-in-Picture**: Universele ondertitelondersteuning toegevoegd voor de plyr-speler.
- **Pagina actief houden**: Verbeterde functionaliteit om tabbladen actief te houden.
- **Stijl van groepstabbladen**: De stijl van tabbladen binnen groepen gewijzigd.
- **Menuvolgorde**: De volgorde van items in het tabbladmenu aangepast.

### Opgelost
- **Picture-in-Picture**: Een probleem opgelost waarbij de titel niet veranderde na het wisselen van video's in de Picture-in-Picture-speler.
- **Aangepaste groepstoewijzingen**: Een probleem opgelost waarbij wijzigingen in aangepaste groepstoewijzingen voor websites niet onmiddellijk van kracht werden wanneer de optie "Sitegroepering onthouden" was ingeschakeld in de instellingen voor Geavanceerde Tabbladgroepen. Dit is opgelost om wijzigingen direct toe te passen zonder dat een herstart nodig is.

----

## [2.10.2] - 2024-10-07

- Probleem opgelost waarbij danmaku (bullet comments) zouden stoppen of verdwijnen op sommige websites na het wisselen van pagina's (pagina verberg gebeurtenis)
- HTML5 videobesturingselementen verborgen

----
## [2.10.1] - 2024-10-05

### Opgelost
- Probleem opgelost waarbij sneltoetsgebeurtenissen herhaaldelijk werden geactiveerd bij het achtereenvolgens afspelen van meerdere video's
- Probleem opgelost waarbij de speler in bepaalde situaties niet kon worden hersteld
- Probleem opgelost waarbij de afspeelvoortgangsbalk niet goed werkte bij gebruik van de Picture-in-Picture-modus
- Probleem opgelost waarbij het wisselen van tabbladen een Picture-in-Picture-detectiemelding zou activeren na het navigeren van een pagina met een video naar een pagina zonder video in hetzelfde tabblad
- Probleem opgelost waarbij het Picture-in-Picture-venster niet sloot bij het verlaten van de Picture-in-Picture-modus met jwPlayer
- Probleem opgelost waarbij een onjuist adres de pagina liet crashen bij het instellen van een achtergrondafbeelding

----
## [2.10.0] - 2024-10-01

### Toegevoegd
- **Document Picture-in-Picture**: Introductie van Advanced Picture-in-Picture, beschikbaar voor gratis proefversie vóór de officiële release van de premiumversie van de extensie. Wanneer ingeschakeld, heeft het voorrang op de standaard Picture-in-Picture. Als de huidige pagina het niet ondersteunt, wordt de standaardmodus gebruikt. Advanced Picture-in-Picture beschikt over een aangepaste videospeler met functionaliteiten zoals:
  * **Video afspelen/pauzeren** (Spatie of K)
  * **Volume aanpassen** (Pijl omhoog/omlaag)
  * **Video dempen/dempen opheffen** (M)
  * **Video vooruit/terugspoelen** (Pijl links/rechts of muiswiel)
  * **Video 5 seconden vooruit/terugspoelen** (Pijl links/rechts)
  * **Video 10 seconden vooruit/terugspoelen** (J/L)
  * **Volgende video afspelen** (Shift + N)
  * **Vorige video afspelen** (Shift + P)
  * **Ondertitels weergeven** (ondersteund op sommige websites zoals youtube.com, vimeo.com, tver.jp, enz.) (C)
  * **Barrage weergeven** (ondersteund op sommige websites zoals nicovideo.jp, bilibili.com, enz.) (D)
  * **Picture-in-Picture afsluiten** (Esc)
  * **Video verbergen/tonen en afspelen/pauzeren wisselen** (Q)
  * **Volledig scherm wisselen** (F)
  * **Afspeelsnelheid aanpassen** ( > of <)
  * **Naar begin/einde van video gaan** (Home/End)
  * **Naar percentage van video gaan** (0-9)
  * **Venster aanpassen aan videomaat** (W)
  * **Picture-in-Picture wisselen vanaf hoofdpagina** (Alt + P)
  
  > Als de websites die u vaak bezoekt ondertitels of barrage ondersteunen, kunt u een [probleem: Advanced Picture-in-Picture](https://github.com/RabbitPair/colorful_sidepanel_tabs_extension/issues/new?assignees=&labels=&projects=&template=Advanced-Picture-in-Picture.md&title=) indienen, en we zullen het zo snel mogelijk aanpassen. Houd er rekening mee dat sommige websites regionale beperkingen kunnen hebben, waarvoor aanvullende informatie nodig is.
- **Sneltoets voor Picture-in-Picture**: Er is een nieuwe sneltoets Alt+P toegevoegd om de Picture-in-Picture-modus snel te wisselen. Dit stelt gebruikers in staat om eenvoudig video's naar de Picture-in-Picture-weergave te schakelen zonder de muis te gebruiken, wat de productiviteit en multitasking-mogelijkheden verbetert.
- **Picture-in-Picture wisselen in onderste navigatiebalk**: U kunt nu een Picture-in-Picture-wisseloptie toevoegen aan de onderste navigatiebalk. Dit kan worden geconfigureerd in de uiterlijkinstellingen onder "Toon onderste navigatiebalk" - "Configureren".
- **Tabbladen sorteren op URL**: Er is een nieuwe menuoptie "Tabbladen sorteren op URL" toegevoegd aan het "Meer"-menu.
- **Tabbladgroep inklapgedrag**: Er is een nieuwe optie "Tabbladgroep inklapgedrag" toegevoegd aan het menu "Geavanceerde Tabbladgroep". U kunt het gedrag van het inklappen van tabbladgroepen in de browser wijzigen. De opties omvatten: 'Toon huidige groep en klap andere groepen in', 'Alle groepen uitvouwen' en 'Standaardinstellingen van de browser gebruiken'.
- **Site-instellingen**: Drie nieuwe opties zijn toegevoegd aan de site-instellingen:
  * **Actie voor Picture-in-Picture-beperking**: Configureer de actie voor Picture-in-Picture-beperkingen.
  * **Automatisch Picture-in-Picture inschakelen**: Automatisch de Picture-in-Picture-modus inschakelen wanneer er een video aanwezig is bij het betreden van de pagina.
  * **Ondertitelinstellingen**: Configureer de CSS-selectoren voor het ondertitelelement en het bovenliggende element op de pagina.

### Veranderd
- Wanneer het zijpaneel-tabblad niet is geopend, wordt bij ingeschakelde optie "Picture-in-Picture bij tabbladwissel" (standaard ingeschakeld) automatisch de Picture-in-Picture-modus ingeschakeld (Belangrijke herinnering: Gebruikersinteractie is vereist, zoals klikken op de pagina die de video afspeelt om de gebruikersinteractie te activeren).
- Bij het sluiten van de zijbalk van de pagina wordt deze nu verwijderd in plaats van verborgen. Het verschijnt pas weer na het vernieuwen van de pagina.

### Opgelost
- Opgelost het probleem waarbij de Snelle Toegang-lijst meerdere URL's niet verwerkte.

----

## [2.9.0] - 2024-09-15

- Toegevoegd **Tabbladen Wissen**: Sla een momentopname op en sluit alle tabbladen behalve het actieve tabblad. Herstel ze vanuit recent gesloten tabbladen of momentopnamen.
- Toegevoegd **Automatisch Activeren van Tabblad Groepering**: Maak automatisch een nieuwe groep aan bij het openen van een nieuw tabblad. Volgende tabbladen die vanuit dit tabblad worden geopend, zullen zich bij de groep voegen.
- Toegevoegd **Lijst Verticale Afstand**: Nieuwe optie in Geavanceerde Tabblad Groep instellingen om de verticale afstand voor lijstitems aan te passen.
- Toegevoegd **Meerdere URL's Toevoegen aan Snelle Toegang**: Hiermee kunt u groepen toevoegen en meerdere tabbladen selecteren om op te slaan in Snelle Toegang.
- Toegevoegd **Snelle Toegang Item Afstand**: Stel verticale/horizontale afstand in voor Snelle Toegang items op de optiepagin.


---
## [2.8.0] - 2024-09-12

### Toegevoegd
- Toegevoegd **Tab Geschiedenis**: Nu kunt u eenvoudig zien welke websites zijn geopend onder hetzelfde tabblad. Klik links om de website te openen in het huidige tabblad, klik in het midden of Ctrl+klik links om de website te openen in een nieuw tabblad. Voor meer details, raadpleeg de opties pagina.
- Toegevoegd **Aangepaste groepsnamen**: In de opties pagina - Geavanceerde Tab Groep, kunt u hier enkele vooraf gedefinieerde groepen toevoegen, zodat u ze snel kunt selecteren wanneer u tabbladen aan een groep moet toevoegen. We hebben al enkele groepsnamen vooraf ingesteld, die u kunt aanpassen of verwijderen naar uw behoeften.
- Toegevoegd **Gebruik bladwijzermapnaam als groepsnaam**: In de opties pagina - Geavanceerde Tab Groep, is een nieuwe optie toegevoegd. Als de geopende website een bladwijzer is, wordt deze automatisch toegevoegd aan de groep en wordt de groepsnaam de naam van de bladwijzermappen.
- Toegevoegd **Tab Index**: In de opties pagina, wanneer ingeschakeld, wordt de tab-index weergegeven naast de titel, waardoor het eenvoudig is om het tabblad actief te maken met behulp van [Ctrl+nummer] op Windows of [cmd+nummer] op Mac. Voorbeeld: 1. stackoverflow.com 2. youtube, zodat het gemakkelijk is om Ctrl + 2 op Windows of cmd + 2 op Mac te gebruiken om naar youtube te gaan
- **Geoptimaliseerde site-instellingen**: Verbeterde optie om achtergrondkleur en lettertypekleur voor sites in te stellen.

### Veranderd
- Bij het controleren van bladwijzers, toestaan bijwerken van doorgestuurde URL's. Als de URL niet toegankelijk is, toon foutcodes: Succesvolle reacties (200 – 299), Doorverwijzingsberichten (300 – 399), Clientfoutreacties (400 – 499), Serverfoutreacties (500 – 599). Voor meer details, zie: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Opgelost
- Opgelost het probleem waarbij het pop-upvenster voor bladwijzerwijzigingen niet verdween

---
## [2.7.0] - 2024-09-05
### Toegevoegd
- Toegevoegd **bladwijzerbeheer**: Volledig uitgeruste bladwijzerbeheerfunctionaliteit toegevoegd
- Toegevoegd **Tab-navigatiebalk**: opties in uiterlijk, weergave: tabbladen, bladwijzers, geschiedenis, recent gesloten tabbladen, leeslijst en snelle toegang in het zijpaneel
- Toegevoegd **Tabblad aan groep toevoegen** menu: tabbladen toevoegen aan een nieuwe groep of een bestaande groep
- Zoekwoordmarkering toegevoegd
- Premium Edition-reservering toegevoegd
### Veranderd
- Aangepaste Cookie-, Leeslijst- en bladwijzerrechten naar optionele rechten, waarvoor gebruikersautorisatie nodig is voor gebruik
### Verouderd
- **Optiepagina - Geschiedenis - Weergeven in zijpaneel**: Deze optie is vervangen door *Tab-navigatiebalk* en zal binnenkort verouderd zijn

### Opgelost
- Opgelost het probleem waarbij de uitbreidingsknop niet verscheen bij het eerste klikken op de zijbalk
- Opgelost het probleem waarbij het opnieuw openen van de browser en het klikken op het extensie-icoon opnieuw selecteren tussen pop-up of zijbalk vereiste
- Opgelost het probleem waarbij de grootte van het vastgezette tabblad-icoon en het snelle toegang-icoon inconsistent waren

---

## [2.6.1] - 2024-08-30

### Veranderd
- Geoptimaliseerde menuweergavemethode, verbeterde foutmeldingen
- Meer compatibiliteit toegevoegd voor Chromium-gebaseerde browsers

---

## [2.6.0] - 2024-08-28
### Toegevoegd
- Toegevoegd **Tabmenu Zoom**: Een zoomfunctie is toegevoegd aan het tabmenu, waarmee u het zoomniveau vrij kunt aanpassen van 1% tot 1000%.

### Veranderd
- Snelle toegang is verplaatst naar een apart menu-item.
- Geoptimaliseerde sleep-en-neerzet sortering

### Opgelost
- Opgelost een probleem waarbij sommige gebieden niet veranderden na het wijzigen van de letterkleur.

### Verouderd
- **Snelle toegang in tabmenu**: Snelle toegang is verplaatst naar een apart menu-item. De optie in het tabmenu zal binnenkort verouderd zijn (de functionaliteit blijft hetzelfde).

### Verwijderd
- De zoomoptie uit de site-instellingen verwijderd omdat het aanpassen van de zoom in het menu geen intuïtieve preview van de wijzigingen gaf. De zoomfunctie is verplaatst naar het tabmenu voor realtime preview.

---

## [2.5.2] - 2024-08-27

### Opgelost

- Opgelost het probleem waarbij opgeslagen achtergrondafbeeldingen verloren gingen na het opnieuw opstarten van de applicatie
- Opgelost het probleem waarbij het sluiten van alle tabbladen van dezelfde site in alle vensters mislukte
- Crash opgelost bij het uitschakelen van DnD

---

## [2.5.0] - 2024-08-25

### Toegevoegd

- Ondersteuning voor sleep-en-neerzet sortering van tabbladen en groepen in tabvolgorde, en synchronisatie met Chrome
- Synchroniseer groepsuitbreidingsstatus met Chrome

### Opgelost
- Opgelost het probleem waarbij het uploaden van een te groot achtergrondafbeeldingsbestand een QUOTA_BYTES quota overschreden fout veroorzaakte
- Opgelost het probleem waarbij het weergeven van alle venstertabbladen een fout veroorzaakte en groeperen op site mislukte

---

## [2.4.0] - 2024-08-20

### Toegevoegd
- Toegevoegd **Achtergrondafbeelding uploaden**: U kunt een afbeelding van uw lokale apparaat uploaden om als achtergrond te gebruiken.
- Toegevoegd **Aangepaste achtergrondkleur**: Ondersteunt nu aangepaste achtergrondkleuren, en u kunt ook een kleur kiezen om een mooie gradient te genereren

### Veranderd

- **letterkleur**: De letterkleur verandert automatisch naar zwart of wit op basis van de dominante kleur van de achtergrond of achtergrondafbeelding. Als de afbeelding groot is, kan het enige tijd duren om de achtergrond toe te passen, wat normaal is.

### Opgelost
- Opgelost het probleem waarbij sommige gebieden niet veranderden na het wijzigen van de letterkleur

### Verouderd
- **Achtergrondstijl lijst**: Deze functie stelt de achtergrondstijl in voor elke lijst, met enkele ingebouwde gradientkleuren. Echter, met de release van aangepaste achtergrondkleuren, is zijn missie voltooid en zal het binnenkort worden verwijderd.

---

## [2.3.0] - 2024-08-16

### Toegevoegd
- Toegevoegd **Zijbalk op pagina's**: De pagina-zijbalk stelt u in staat een zijbalk in te voegen in de webpagina's die u bekijkt zonder de browserzijbalk te openen om tabbladen te beheren. Dit is een zeer nuttige functie voor gebruikers met kleinere schermresoluties die de browserzijbalk te breed en niet aanpasbaar vinden. Echter, vanwege enkele beperkingen, biedt de pagina-zijbalk slechts zeer beperkte functionaliteit. Wanneer deze functie is ingeschakeld, kunt u met de muis over de rand van het venster bewegen om de zijbalk tevoorschijn te halen.

### Verwijderd
- Verwijderd **Zwevende bal**

---

## [2.2.0] - 2024-08-14

### Toegevoegd
- Nieuw tabmenu **Tabblad actief houden**: Houd het tabblad actief zodat het niet automatisch wordt verwijderd.

### Veranderd
- Geoptimaliseerde prestaties en verminderde bundelgrootte.

---

## [2.1.0] - 2024-08-10

### Toegevoegd
- Sla automatisch venster-, groep- en tabbladmomentopnamen op. Na het opnieuw opstarten van de browser, als er slechts één venster open is en minder dan 5 nieuwe tabbladen zijn geopend, zal een toast vragen om het laatst opgeslagen venster- en tabbladinformatie te herstellen wanneer de zijbalk wordt geopend.

### Veranderd
- Geoptimaliseerde opslaggegevens voor snelle toegang om de toegangstijd te versnellen.

### Opgelost
- Andere kleine problemen opgelost.

---

## [2.0.1] - 2024-08-09

### Opgelost
- Opgelost het berichtformaat voor succesvolle momentopname-import.
- Opgelost het probleem waarbij dubbele importen herhaalde snelle toegang-items veroorzaakten.

---

## [2.0.0] - 2024-08-08

### Veranderd
- De extensie hernoemd van "Colorful Side Panel Tabs" naar **"VertiTab - Side Panel Vertical Tabs"**.

### Toegevoegd
- Momentopnamen: Een een-klik opslaan browser tabblad momentopname functie toegevoegd. U kunt momentopnamen opslaan voordat u de browser sluit en deze snel herstellen de volgende keer dat u deze opent. Momenteel kunnen maximaal 50 momentopnamen worden opgeslagen.
- Verbeterde onderste navigatiebalk: Toegang tot meer functies vanaf de onderste navigatiebalk, zoals bladwijzers, geschiedenis, recent gesloten tabbladen, leeslijst, snelle toegang, nieuw tabblad openen, momentopname maken, zoeken, groepen samenvouwen, enz.
- Bijgewerkte import/export functionaliteit: Verbeterde import- en exportopties om tabbladen beter te beheren op verschillende apparaten.

### Opgelost
- Bugfixes en stabiliteitsverbeteringen.

---

## [1.3.3] - 2022-08-04

### Toegevoegd
- **linkInstellingen**: Site-instellingen bevatten nu een nieuwe optie waarmee u regels kunt toevoegen om te bepalen of sitelinks in het huidige tabblad of in een nieuw tabblad worden geopend.

---

## [1.3.2] - 2024-08-02

### Opgelost
- Opgelost het probleem dat klikken op de middelste muisknop om het tabblad te sluiten niet werkte.

---

## [1.3.1] - 2024-08-01

### Veranderd
- Geoptimaliseerde lay-out van snelle toegang en ondersteuning voor sleep-en-neerzet sortering toegevoegd.
- Verbeterde logica voor het uitbreiden van alle groepen en het onthouden van hun status.

### Opgelost
- Opgelost het probleem waarbij het importeren van snelle toegang-gegevens mislukte wanneer het zijpaneel niet open was.
- Opgelost het probleem waarbij pictogrammen verkeerd waren uitgelijnd in de groepsweergave.
- Andere kleine problemen opgelost.

---

## [1.3.0] - 2024-07-30

### Toegevoegd
- **Importeren/Exporteren**: Exporteer gebruikersvoorkeuren, snelle toegang, website-instellingen en recent gesloten tabbladen gegevens, en importeer ze in een andere browser om extensiegegevens te synchroniseren.
- **Selecteer snelle toegang uit geschiedenis**: U kunt de meest bezochte websites uit de geschiedenis zoeken en toevoegen aan de snelle toegang.
- **Meer opties in de werkbalk**: Voeg meer opties toe aan de werkbalk. U kunt het label op de werkbalk verbergen en bepalen welke pictogrammen op de werkbalk worden weergegeven.

### Veranderd
- **Zoekvak**: Het zoekvak ondersteunt nu de Enter-toets om trefwoorden in een nieuw tabblad te zoeken. Als er geen overeenkomend tabblad of geschiedenis is na het invoeren van het trefwoord, kunt u op Enter drukken om te zoeken met de standaard zoekmachine.
- **Gegevensinitialisatie**: Pas de timing van gegevensinitialisatie aan en optimaliseer herhaald renderen veroorzaakt door gegevenswijzigingen.
- **Changelog URL**: Update de changelog URL naar de release URL op GitHub.
- **Lay-out optimalisatie**: Optimaliseer lay-outwijzigingen wanneer de venstergrootte verandert.
- **Foutlogboeken opnemen**: Gebruik Sentry om foutlogboeken te verzamelen. Wees gerust, deze functie verzamelt uw privégegevens niet.

### Opgelost
- **Tooltip positie fout**: Opgelost het probleem waarbij de tooltip flitste bij het wisselen van thema's en weergaven in de werkbalk.
- **Onderste navigatie**: Opgelost het probleem waarbij de onderste navigatie de lijst blokkeerde wanneer veel tabbladen open waren.
---

## [1.2.3] - 2024-07-23

### Opgelost
- Opgelost onjuiste lijst scroll hoogte berekening wanneer vastgezette tabbladen en snelle toegang pictogrammen meer dan 1 rij overschrijden.

### Veranderd
- Veranderd inactieve tabbladen uitsluiten om vastgezette tabbladen uit te sluiten.
- Veranderd het sluiten van alle weggegooide tabbladen om vastgezette tabbladen uit te sluiten.
- Pas de grootte van vastgezette en snelle toegang pictogrammen aan.

---

## [1.2.2] - 2024-07-19

### Toegevoegd
- Snelle toegang toevoegen: U kunt een tabblad instellen om in Snelle toegang te verschijnen, zodat het gemakkelijk te vinden is. Klik er gewoon met de rechtermuisknop op (of houd het ingedrukt) en selecteer Vastzetten in Snelle toegang. Maak het los wanneer u het daar niet meer nodig hebt door er met de rechtermuisknop op te klikken (of het ingedrukt te houden) en Verwijderen uit Snelle toegang te selecteren. Het verschil met vastgezette tabbladen is dat Snelle toegang de URL opslaat en elke keer dat erop wordt geklikt een nieuw tabblad opent.

### Veranderd
- Vastgezette tabbladen tonen alleen pictogrammen om te voorkomen dat ze per ongeluk worden aangeklikt en vervolgens worden losgemaakt.
- Pas de grootte van vastgezette tabbladpictogrammen aan.

---

## [1.2.1] - 2022-07-17

### Toegevoegd
- Voeg nieuw menu toe aan onderste navigatie: inactieve tabbladen weggooien.
- Voeg nieuw menu toe aan onderste navigatie: sluit alle weggegooide tabbladen.

### Veranderd
- Wijzigingen in het onderste navigatiemenu "Groeperen op site" hebben alleen invloed op het huidige venster.

### Opgelost
- Opgelost het probleem waarbij de UI zou springen vanwege hoogte-inconsistentie bij het wisselen van actieve tabbladen in de lijst.

---

## [1.2.0] - 2024-07-16

### Toegevoegd
- Voeg Site Configuraties toe: Pas site-specifieke instellingen aan, zoals het uitschakelen van Picture-in-Picture-modus, het uitschakelen van automatische wegwerpmodus en meer.

### Opgelost
- Los Auto Creëren of Meedoen met Zelfde Domein Groep op: Opgelost een probleem waarbij het automatisch creëren of meedoen met dezelfde domeingroepen niet werkte wanneer een tabblad werd bijgewerkt.
- Los Pagina Niet Ontvangen Configuratie Update Berichten op: Zorg ervoor dat pagina's correct configuratie-updateberichten ontvangen.
- Los Andere Bugs op: Behandelde verschillende andere bugs om stabiliteit en prestaties te verbeteren.

### Veranderd
- Voeg Optie toe om Sluitknop te Tonen bij Hover: Toegevoegd een optie om de sluitknop alleen weer te geven wanneer u over een tabblad zweeft.

---

## [1.1.0] - 2024-07-13

### Toegevoegd
- Voeg Prestatie Opties toe: Introduceer nieuwe prestatie-instellingen om uw browse-ervaring aan te passen en te verbeteren.
- Voeg Scroll naar Actieve Tabblad Pictogram toe: Navigeer eenvoudig naar het actieve tabblad met een nieuw scroll-naar-actieve tabblad pictogram.
- Voeg Tabbladen Sorteren op Domein toe: Organiseer uw tabbladen op domein met een nieuwe sorteermogelijkheid.
- Dempen Alle Tabbladen die Geluiden Maken: Dempen snel alle tabbladen die geluiden afspelen voor een stillere browse-ervaring.

### Veranderd
- Verwijder Herstel Pictogram: Het herstelpictogram is verwijderd en vervangen door lijsttekst opaciteit ingesteld op 0,5 voor een schonere uitstraling.

### Verouderd
- Verwijder Sleep-en-Neerzet Sortering: De huidige oplossing voor sleep-en-neerzet sortering heeft prestatieproblemen en is tijdelijk verwijderd.

---

## [1.0.4] - 2024-07-09

### Toegevoegd
- Sleep-en-Neerzet Sortering voor Tabbladen: Rangschik uw tabbladen eenvoudig opnieuw met sleep-en-neerzet functionaliteit.

### Veranderd
- Optimaliseer Pagina Laadsnelheid: Verder verbeterde pagina laadsnelheid voor een nog soepelere browse-ervaring.

---

## [1.0.3] - 2024-07-05

### Opgelost
- Los Gemengde Weergave Menu Fout op: Opgelost een probleem waarbij het gemengde weergave menu fouten vertoonde.

### Veranderd
- Optimaliseer Tabblad Groep Domein Menu: Verbeterde het tabblad groep domein menu voor betere organisatie en bruikbaarheid.
- Optimaliseer Tabblad Padding: Aangepaste tabblad padding voor een meer gestroomlijnde en visueel aantrekkelijke lay-out.

---

## [1.0.2] - 2024-07-04

### Toegevoegd
- Huidige Actieve Tabblad Indicator: Identificeer eenvoudig het actieve tabblad met een nieuwe visuele indicator.
- Aangepaste Letterkleur: Personaliseer uw interface door een aangepaste letterkleur in te stellen.

### Veranderd
- Optimaliseer Laadsnelheid: Verbeterde laadsnelheid voor een snellere en soepelere gebruikerservaring.

### Standaardinstellingen
- Stel Standaard Niet in om Kleurmodus te Gebruiken: De standaardinstelling gebruikt nu de enkelkleurmodus voor een vereenvoudigde uitstraling.

---

## [1.0.1] - 2024-07-02

### Toegevoegd
- Volledige Geschiedenis Record per Tijd Bereik: Toegang tot en beheer uw browsegeschiedenis met gedetailleerde records gesorteerd op tijdsbereik.
- Enkelkleurmodus voor Lijst: Introduceer een enkelkleurmodus voor een vereenvoudigde en consistente lijstweergave.

### Veranderd
- Volledige Audio Voortgangsbalk Update Timing: Verbeterde de nauwkeurigheid van audio voortgangsbalk updates voor een soepelere multimedia-ervaring.
- Geoptimaliseerde Lijst Pictogram Acquisitie Methode: Verbeterde de methode voor het verkrijgen van lijstpictogrammen, resulterend in snellere en betrouwbaardere pictogramladen.

### Opgelost
- Los Onjuiste Activatiestatus Weergave Probleem op in Meerdere Vensters: Opgelost een probleem waarbij de activatiestatus onjuist werd weergegeven wanneer meerdere vensters open waren.

---

## [1.0.0] - 2024-06-29

### Toegevoegd
- Licht/Donker Modus Schakelaar: Kies tussen lichte en donkere weergavemodi om aan uw voorkeuren te voldoen.
- Aanpasbare Lettergrootte: Pas de lettergrootte aan voor een comfortabelere leeservaring.
- Aanpasbare Interface Lay-out: Personaliseer de interface lay-out volgens uw gebruiksgewoonten.
- Personalisatie Opties: Voeg kleurrijke achtergronden en achtergrondafbeeldingen toe om uw zijpaneel uniek te maken.
- Geavanceerd Tabbladbeheer: Miniatuurvoorbeelden, rijke sorteer- en weergaveopties, en een uitgebreid actiemenu voor efficiënt tabbladbeheer.
- Zoekfunctionaliteit: Zoek snel naar recent gesloten tabbladen of blader door uw geschiedenis om te vinden wat u nodig hebt.
- Picture-in-Picture Modus: Schakel naadloos over naar Picture-in-Picture modus bij het wisselen van tabbladen of scrollen door pagina's.
- Automatische Groepering: Maak automatisch groepen aan of sluit aan bij groepen op basis van hetzelfde domein voor betere organisatie.
- Lees Voortgangsbalk: Volg uw leesvoortgang in real-time om te weten hoe ver u hebt gelezen.
- Afspelen Voortgangsbalk: Beheer multimedia afspelen met opties voor vooruitspoelen, terugspoelen, volumeregeling en afspeelsnelheid aanpassing.
