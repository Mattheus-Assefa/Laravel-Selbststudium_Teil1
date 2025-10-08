# Laravel-Selbststudium_Teil 1
## 1.1 PHP (Hypertext Preprocessor)
  1. Was ist PHP und wofür wird es hauptsächlich verwendet?
     - Es handelt sich bei PHP um eine Skriptsprache, die in einigen Details mit Programmiersprachen wie C oder Perl vergleichbar ist.
     - Der wichtigsten Einsatzbereiche von PHP sind:
         - dynamische Webinhalte,
         - Serverseitige Verarbeitung
     - PHP ist Server-Side, dass heißt die Daten werden im Server verarbeitet anstatt am Client Computer.
  2. Welche sind die wichtigsten Datentypen in PHP?
     - String
         - ```$Username = $_POST['name'];```
     - Integer
         -  ```$Quantity = $_POST['quantity'];```
     - Float
         - ```$Full_Price = $Price * $Quantity * $Taxes;```
     - Boolean & NULL
         - ```$Adult = true;``` or ```$Adult = null;```
  3. Wie funktioniert die Einbindung von PHP-Code in HTML?
     - So sehen PHP-Tags aus: ```<?php ?>``` wenn man diese in ein file einbaut, kann man in dem file php code benutzen.
     - PHP erkennt die Opening und Closing Tags und limitiert die Verarbeitung vom PHP Code auf was dazwischen ist,<br> alles außerhalb wird vom PHP Parser ignoriert.
  4. Was sind PHP-Superglobals?
     - GLOBALS ```$GLOBALS['x']```
         - Mit GLOBALS kannst du auf Variablen zugreifen, die außerhalb der Scope sind.
     - POST ```$_POST['x']```
         - Mit POST kannst du auf Variablen zugreifen, die von einer HTTP POST method kommen.
     - GET ```$_GET['x']```
         - Mit GET kannst du auf Variablen zugreifen, die von einer HTTP GET method kommen.
     - REQUEST ```$_REQUEST['x']```
         - Mit REQUEST kannst du auf Variablen zugreifen von GET, POST und COOKIE Superglobals.
     - FILES ```$_FILES['x']```
         - Mit FILES können die Daten von Dateien die upgeloaded werden zugegriffen werden.
  5. Welche Vorteile bietet PHP für die Webentwicklung?
     - Problem Lösung
     -   Man hat eine einfache Zeit Lösungen zu googlen, da soviele es benutzen.
     - Open Source
       - Da PHP Open Source ist wird die Sicherheit überprüft und PHP immer erweitert.
     - Datenbankunterstützung
       - PHP ist sehr flexibil und unterstützt viele Datenbanken.
     - Plattformkompatibilität
       - PHP unterstützt viele Betriebsysteme und arbeitet nahtlos mit Webservern zusammen.
## 1.2 Laravel Framework
  1. Was ist Laravel und auf welcher Architektur basiert es?
     - Laravel ist ein Open Source PHP Framework.
     - Laravel folgt der MVC Architektur.
     - Laravel MVC
       - Laravel erstellt eine View die der User sehen kann und mitdem der Username anfragen stellen kann.
       - Controller können Daten überprüfen, gewisse Daten fordern und REST Befehle weiterleiten.
       - Model nimmt, bearbeitet, erstellt oder löscht Daten aus der Datenbank.
  2. Was ist der Unterschied zwischen Laravel und reinem PHP?
     - Entwicklungsgeschwindigkeit
       - Mit PHP Projekten muss man vieles selber schreiben, während bei Laravel viel schon vorgemacht wurde.
       - Laravel ist einfacher zu skalieren.
       - Laravel hat einen build-in Sicherheitsmechanismus.
  3. Wie funktioniert das Routing in Laravel?
     - Alle Routes werden im Route File definiert, auf die kann ein Laravel Projekt zugreifen.
     -
## 1.4 Laravel Herd
  1. Was ist Laravel Herd und für welche Betriebsysteme ist es verfügbar?
     - Laravel Herd ist ein Tool von Laravel selbst.
     - Laravel Herd unterstützt Windows und macOS.
     - Laravel Herd erstellt eine entwicklungsumgebung für Laravel.
  2. Was sind die wichtigsten Features von Laravel Herd?
     - Zero Configuration
     - Built-in SSL
     - Schnelles Setup
     - Robuste Performance
     - Support für nicht Laravel Projekte
  3. Wie erstellen Sie ein neues Laravel Projekt in Laravel Herd?
     - Man installiert sich Laravel Herd (Herd)
     - Dann geht man zu Sites
     - Dann drückt man auf Add Site
     - Dann drückt man auf "New Laravel project"
     - Dann kann man sich entscheiden was man für ein Starter Kit haben möchte oder ob man keines haben möchte (Die Entscheidung liegt bei einem selbst)
     - Dann muss man einen Project Name geben und dann hat man schon das Projekt.
# Laravel-Selbststudium_Teil 2
## Fehler die passiert sind
  1. failed to listen on 127.0.0.1:8000
     - Um es zu lösen ging ich [hier](https://stackoverflow.com/questions/63955357/laravel-failed-to-listen-on-127-0-0-18000-reason)
       - Ich habe das php.init file von der aktuellen php version bearbeitet.
       - variables_order = "GPCS"
  2. HTML wird nicht vorgeschlagen
     - Um es zu lösen ging ich [hier](https://github.com/laravel/vs-code-extension/issues/69)
       - Ich habe das File settings.json gesucht und habe das hier eingebaut:
         ```
         "emmet.includeLanguages": {
           "blade": "html"
         }
         ```
  3. 








Sources: <br>
[Was ist PHP?](https://www.hostpress.de/blog/was-ist-php-und-wofuer-wird-es-verwendet/)<br>
[Server-Side vs. Client-Side](https://a-digital.one/magazin/server-side-vs-client-side-was-es-bedeutet-und-wie-es-genutzt-wird/)<br>
[PHP Data Types](https://www.w3schools.com/php/php_datatypes.asp)<br>
[PHP Tags](https://www.php.net/manual/en/language.basic-syntax.phptags.php) <br>
[PHP Superglobals](https://www.geeksforgeeks.org/php/php-superglobals/)<br>
[Vorteile von Open Source](https://www.reddit.com/r/explainlikeimfive/comments/1d6g75d/eli5_what_are_the_benefits_of_opensource_software/)<br>
[Plattformkompatibiltät](https://prehost.com/de/what-is-php/)<br>
[Laravel in Wikipedia](https://de.wikipedia.org/wiki/Laravel)<br>
[Laravel vs Core PHP](https://dotbite.at/blog/laravel-vs-core-php-the-winner-is-pretty-clear-in-2025)<br>
[What is Laravel Herd and the differences between other tools](https://medium.com/@thomas-emad/what-is-laravel-herd-and-is-it-worth-replacing-laragon-for-it-fd63f083e486)<br>
[What is Laravel Herd](https://arjunamrutiya.medium.com/what-is-laravel-herd-a-detailed-guide-with-examples-5c65049dbd5c)<br>








