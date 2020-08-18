# HG-Datenbanken Webservices Information
Infos und Demos für Webservices

## Aufruf der Webservices
Der Aufruf kann mit dem Programm **Curl** simuliert werden. Das Programm Curl ist in Windows 10 bereits enthalten, bei älteren Windows Versionen muss das Programm heruntergeladen werden. Curl ist Open Source und kann von der Website https://curl.haxx.se/ für diverse Betriebssysteme heruntergeladen werden.

## Aufrufe der Webservices
Die Dokumentation zu den Webservives ist auf unter der Uri https://db.hgkv.at/apiDocumentation/index.html unter dem Punkt *HgkvService400* erreichbar, die anderen Menüpunkte sind nicht für die Services verwendbar.

### Beispiel eines Aufrufs 
curl --user user:password -x GET "https://db.hgkv.at/api/service/400/Ping" -H "accept: application/xml"

#### Info zum Aufruf
* curl 
* --user user:password hier werden die von HG-Datenbanken bereitgestellten Anmeldeinformationen angegeben
* -X den folgenden Aufruf verwenden
* GET HTTP Kommando (GET, POST, PUT...)
* https://... Uri 
* "accept: application/json" Information wie die Daten geliefert werden, in diesem Fall json, kann mit "accept: application/xml" auf XML umgestellt werden.

#### Testen der Verbindung
Falls es zu Fehlermeldungen kommt können sie den oben genannten Aufruf *Ping* auch ohne Anmeldung verwenden um zu überprüfen ob sie die Services generell erreichen können.
