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

###Welche Programmiersprache nutzt das Programm?

Der Scraper ist in Python geschrieben

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

###Unter welcher Lizenz steht der Quellcode?

http://creativecommons.org/publicdomain/zero/1.0/deed.de