# Onlineshops

## Allgemeines

- Die installation läuft immer im selben Ordner. Ein nachträgliches ansehen ist nicht möglich. Läuft dann alles unter [shop.computer-extra.com](shop.computer-extra.com)
- Ordner auf dem Webspace ist "magento"

## Contao mit Isotope Ecommerce

Infos: [Contao](https://contao.org/de/) - [Isotope Ecommerce](https://www.isotopeecommerce.org/de/)

### Ablauf der Installation

- Installation per .phar Datei (Composer)
- Aufruf der installation per `/contao-manager.phar`
- Benötigt Composer installiert auf dem Webspace.
- Installation auch per SSH möglich.
- Domain muss nach der Installation auf einen Unterordner verweisen. In diesem Fall `/web`

### Funktionen im Test

- [ ] Import von CSV Dateien

### Aufgetretene Probleme

- Installation per Manager hat nicht funktioniert und gibt nur noch einen Serverfehler 500 zurück.
- zweiter Versuch direkt mit Composer per SSH
- Installation lief durch.
- Bei der Konfiguration kommt "Es ist ein Fehler aufgetreten" laut dem Log wird MariaDB nicht unterstützt. Dementsprechend kann Contao nicht bei uns im Hosting verwendet werden.

## Zen Cart

Infos: [Link](https://www.zen-cart-pro.at/)

### Ablauf der Installation

- Installations Archiv auf Deutsch mit deutscher Installationsanleitung.
- Einfache installation

### Funktionen im Test

- [ ] Import von CSV Dateien

### Aufgetretene Probleme

- Kein Import Modul vorhanden.

## Open Cart

Infos: [Link](https://www.opencart.com/)

### Ablauf der Installation

- Große installationsdatei (> 12.000 Dateien)
- Alles Englisch

### Funktionen im Test

- [ ] Import von CSV Dateien

### Aufgetretene Probleme

- Keine Deutsche Sprachdatei verfügbar.
- Keine Import Funktion

## OSCommerce

Infos: [Link](https://www.oscommerce.com/)

### Ablauf der Installation

- Installation durch ZIP Package. ZIP auf Webspace laden, wird durch php Skript entpackt.
- Installation komplett auf Englisch
- Super unübersichtliches Backend.
- Scheinbar keinerlei Möglichkeit eine deutsche Sprachdatei zu installieren.
- Alle voreinstellungen sind für einen UK Shop.

### Funktionen im Test

- [x] Import von CSV Dateien (XML ist auch möglich)

### Aufgetretene Probleme

- Ist alles auf den UK Markt ausgelegt.
- Komplett unübersichtlich.

## Cubecart

Infos: [Link](https://www.cubecart.com/)

### Ablauf der Installation

- Einfache und schnelle installation über [/setup](shop.computer-extra.com/setup)
- Admin Panel direkt mit custom Admin URL, damit sie nicht so leicht gefunden werden kann. In diesem Fall: [admin_SM51ej](https://shop.computer-extra.com/admin_SM51ej.php)
- Benutzername für Admin frei wählbar.
- Installation nur auf Englisch möglich.
- Deutsches Sprachpaket kostenfrei nach installierbar. [Deutsch Language Pack
  ](https://www.cubecart.com/extensions/languages/deutsch-language-pack)
- Installation von Plugins durch Tokens
- Backend komplett auf Englisch
- Kein Import von Bildern. Diese müssen manuell hochgeladen und verknüpft werden.

### Funktionen im Test

- [x] Import von CSV Dateien (Nur neue Artikel, keine Möglichkeit für Update)

### Aufgetretene Probleme

- Import scheinbar nur für neue Produkte.
- Export von bestehenden Artikel ist defekt. Die CSV-Datei hat eine falsche Formatierung. Besteht pro Artikel aus 3 Zeilen statt einer.
- Im Admin angelegte Produkte werden nicht im Frontend angezeigt. Auch nicht nach zurücksetzen von Cookies und Cache.
- Es werden Unmengen an Cookies gesetzt. Keine Möglichkeit gefunden, diese abzuschalten oder ein Cookie Banner zwischen zu schalten.
