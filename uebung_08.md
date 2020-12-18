# Übung 8

Stelle deine Band-Website aus [Übung 6](uebung_06.md) online


## Anweisung

Wenn deine Seite in `HTML` und `CSS` fertig gestaltet ist und funktioniert, solltest du sie noch online stellen; ansonsten kann sie niemand ausser dir sehen. Sie liegt ja bisher lediglich als Dateien auf deinem Computer.

Normalerweise hat man keinen eigenen Webserver zuhause, sondern kauft das Hosting als Dienstleistung ein, kostenfrei oder kostenpflichtig. Kostenlose Angebote haben in der Regel irgendwelche Haken. Der Preis für einfaches "Shared Hosting" bewegt sich oft zwischen 2-5 Euro pro Monat für einfache Angebote. Bietet der Provider mehr an, steigt auch der Preis entsprechend.

Für diese Aufgabe kannst du wählen aus:

- [Uberspace](https://uberspace.de/de/) als Provider (Unverbindlich, 1. Monat kostenlos)
- Einem Provider deiner Wahl (siehe Referenzen. Kostet, was es kostet)
- [Github Pages](https://pages.github.com/) (Kostenlos, im Besitz von Microsoft)

### Uberspace

Bei Uberspace kann man sich für einen [kostenlosen Testaccount](https://dashboard.uberspace.de/register?from_beta=1&lang=de) ohne Angabe von Bezahldaten oder Emailadresse registrieren. Nach Ablauf des Testzeitraums kann man entweder einen beliebigen Betrag monatlich bezahlen, oder den Webspace auslaufen lassen (wird dann gelöscht).

Hat man sich registriert, kann man in der Verwaltungsoberfläche unter "Datenblatt" und "Zugänge" die benötigten Verbindungsdaten einsehen (oder setzen! SSH/SFTP-Zugang muss erst angelegt werden!)

Anschliessend kannst du mit einem FTP-Client (Cyberduck, Transmit, Filezilla, etc.) die Daten deiner Website transferieren und unter `deinusername.uber.space` ansehen. Eigene Domainnamen können auf Wunsch bei einem separaten Domain-Hoster (zB. INWX) registriert und mit der IP deines Uberspace verknüpft werden.

**Siehe ausführliche Anleitung hierzu im PDF der Stunde!**

### Eigener Webspace

Du brauchst die (S)FTP-Verbindungsdaten zu deinem Provider, um die Dateien deiner Website mit einem FTP-Programm (Cyberduck, Transmit, Filezilla, etc.) dort hin kopieren zu können. Diese erfährst (oder setzt) du in der Regel in der Verwaltungsoberfläche des Anbieters.

### Github

Github Pages spiegelt einfach die Inhalte eines Git-Repositories deiner Wahl wider. Du brauchst also einen Github-Account und musst deine Dateien dort hin laden. Github hat dafür viele Tutorials und es gibt mehrere Wege, das zu tun.

Liegen deine Dateien in einem Repo deines Accounts, kannst du für dieses Repo unter "Einstellungen" die Ausgabe des `master-branches` als Github Pages aktivieren.

Siehe für eine Anleitung [pages.github.com](https://pages.github.com/)

Prüfe deine Seite (am besten in mehreren Browsern!)


## Dauer und Abgabe

Die veranschlagte Bearbeitungszeit für diese Aufgabe beträgt 7 Tage, bis zur nächsten Kursstunde.  
Bringe die URL (Adresse), unter der deine Seite zu erreichen ist, zum nächsten Kurs mit.

## Referenzen und weiterführende Links

### Programme (FTP-Clients)

- [Transmit](https://panic.com/transmit/) ($45)
- [Forklift](https://binarynights.com/) ($30)
- [Cyberduck](https://cyberduck.io/) (kostenlos)
- [Filezilla](https://filezilla-project.org/) (kostenlos)

### Provider

- [Uberspace](https://uberspace.de/de/)
- [serverprofis.de](https://www.serverprofis.de/)
- [one.com](https://www.one.com/de/)
- [Domainfactory](https://www.df.eu/)
- [Alfahosting](https://alfahosting.de/)

### Separates Domainhosting

- [inwx.de](https://inwx.de/)
- [porkbun.com](https://porkbun.com/)

### Langweilige, riesige Provider

- [1und1 Ionos](https://www.ionos.de/)
- [Strato](https://www.strato.de/)
- [Mittwald](https://www.mittwald.de/)
- [HostEurope](https://www.hosteurope.de/)
