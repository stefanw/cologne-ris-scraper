#Scraper für das Ratsinformationssystem von Köln

Dies ist ein Scraper für die Daten im Ratsinformationssystem (RIS) der Stadt Köln.

Das RIS der Stadt Köln ist unter http://ratsinformation.stadt-koeln.de erreichbar.

Ein Ratsinformationssystem bietet üblicherweise Zugriff auf Informationen zu Sitzungen der Gremien 
(wie z.B. des Stadtrats), die darin behandelten Tagesordnungspunkte, die Anträge 
und Beschlüsse und mehr.

Das Kölner RIS basiert auf der Software SessionNet, die bei vielen Gemeinden, Landkreisen und anderen 
Körperschaften im Einsatz ist. Daher sollte sich dieser Scraper mit leichten Anpassungen auch für andere
SessionNet Instanzen einsetzen lassen.

##FAQ

###Was ist ein Scraper?

Ein Scraper ist ein Programm, dass die Daten aus einer Website extrahiert und in strukturierter Form speichert.

###Welchen Entwicklungsstand hat der Scraper?

Der Scraper kann noch nicht als "fertig" bezeichnet werden.

* Es werden noch nicht alle wesentlichen Daten erfasst.
* Anhänge mit Texten, z.B. TIF-Scans (Faxe) werden nur gespeichert, Volltexte werden jedoch nicht extrahiert.

###Welche Programmiersprache nutzt das Programm?

Der Scraper ist in Python geschrieben.

###Welche Python-Version wird benötigt?

Bisher wurde der Scraper nur mit Python 2.7 getestet.

###Welche Python-Module werden benötigt?

* urllib2
* scrapemark
* mechanize
* MySQLdb
* pdfminer

###Was wird außerdem benötigt?

Zum Speichern der Daten wird aktuell ein MySQL-Server benötigt.

###Wie funktioniert die Installation?

1. Benötigte Python-Module installieren
2. Leere MySQL-Datenbank anlegen
3. Die Datei setup_mysql.sql in der neuen Datenbank ausführen. Damit werden die benötigten Tabellen angelegt.
4. Die Datenbank-Konfiguration in scrape.py anpassen

Danach sollte sich der Scraper mit dem Kommando "python scrape.py" an der Kommandozeile starten lassen.

###Sind die Daten selbst irgendwo verfügbar?

Aktuell noch nicht. Sobald diese eine ausreichende Vollständigkeit erreicht haben, sollen sie irgendwo als MySQL-Dump oder
CSV Download verfügbar gemacht werden. Weitere Informationen werden dann hier zu finden sein.

###Unter welcher Lizenz steht der Quellcode?

http://creativecommons.org/publicdomain/zero/1.0/deed.de
