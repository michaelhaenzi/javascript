Video2Brain JavaScript
======================

###Wo kann ich diese Videos finden?

Hier ist ein explizieter JavaScript Crashkurs für Anfänger: [Video2Brain JavaScript](https://www.video2brain.com/de/videotraining/javascript-crashkurs-2012)

###Was ist JavaScript überhaupt?

Es dient der Aufbereitung von Daten über einen Server. JavaScript gestattet dynamische Aktionen auf einem Webserver. JS ist auf fast allen modernen und neueren Seiten aufzufinden.

###Wo wird JavaScript konkret eingesetzt?

..*Dynamische Manipulation auf Webseiten (Document Object Model)
..*Plausibilitätsprüfung (Prüfung eines Formulars)
..*Senden, Empfangen von Daten (Ajax)
..*Toolbar, dynamische Navigationsleisten und viele andere mehr…

Webseiten bei denen solche Funktionen genutzt werden:

..*Google Map (Zoomen, Verschieben, Route berechnen etc.)
..*Yahoo! (Formular Überprüfung)
..*Andere Seiten

###Was braucht man um Webseiten zu gestalten?

Man sollte einige Grundkenntnisse von HTML und CSS haben. Denn ohne diesen 3er Bund wirkt es steif, langweilig und uninteressant. 
Erforderliche Programme:
Man sollte einen IDE (integrated development environment) besitzen. Da gibt es einige sehr gute im Angebot, wie z.B.: Aptana Studio oder Visual Studio Web Developer.
Neben einem IDE sollte man verschiedene Browser gedownloadet haben. Da man Funktionalität auf den meist genutzten Browsern Test bevor man es öffentlich macht. Dabei eignet sich ganz gut: Firefox, Google Chrome, Internet Explorer, Opera und Safari.

###Firebug, was ist das?

„Firebug“ ist ein Addon was man im Firefox Browser sich gratis Downloaden kann. Es hilft Entwicklern effektiv die Hintergründe der Webseite zu sehen und zu testen. Allgemein empfiehlt sich bei Firefox mit Firebug und beim Internet Explorer eine neu erstellte Seite zu testen. 

###Wie fügt man nun ein JavaScript Skript in eine HTML-Seite ein?

Im Grunde ganz einfach, wie bei CSS. Es gibt 3 Arten beim Einbinden von JS. Durch eine Inline-Referenz, Skript-Container und Externe-Referenz. Diese 3 Arten werden hier ganz kurz erklärt: 

| **JavaScript Einbinden** |   |
| ------------------------ | ------------------- |
|   | **Inline-Referenz** |
| Quellcode	| ```javascript <a href="javascript:alert('Hallo')">Das ist eine Inline-Referenz</a> ``` |
| Beschreibung | Die JavaScript Funktion wird direkt in einem Inline-Element eingebunden. |
|   | **Skript-Container** |
| Quellcode | ```javascript <script> alert("Der interne Skript-Container"); </script> ``` |
| Beschreibung | Hierbei wird einem internen Block-Element eine JavaScript Anweisung zugeteilt. |
|   | **Externe-Referenz** |
| Quellcode | ```javascript <script src="javascript.js"></script> ``` |
| Beschreibung | Man integriert mit scr (source = quelle) eine externe .js Datei. Ist immer vorhanden |

###Datentypen in JavaScript

Es gibt nur 4 Datentypen:
..* number (Nummer: Ganze Zahlen und Kommazahlen)
..* string (Text)
..* boolean (True or False)
..* object (Neues Objekt einfügen)

Diese Einteilung ist sehr weitläufig und daher auch sehr schwer zu kontrollieren. Es gibt noch einen schöneren weg der Deklaration, das ist:
```javascript
var variabelnname = number, string, boolish oder object
```

Zudem ist 'var' (variable) eine nur interne Funktion. 

###Undefined, not defined, null und NaN
Wenn man einem Variablennamen in js nichts zuteilt, also z.B. var a; dann ist jetzt ‚a‘ definiert als ‚undefined‘ welches eine eigene Funktionsnamen in js ist. Wenn man aber eine Variable ausgeben will ohne dass man sie vorher zugeteilt hat, dann gibt es einen Script-Fehler. Dann gibt es noch eine anderen Funktionsnamen ‚null‘ welcher bei der Kontrolle gibt. Wenn man versucht eine Operation von 2 Texten oder keinen Zahlen-Variablen ausgibt. Dann kommt ‚NaN‘ = ‚NotaNumber‘. 

Im JavaScript verwendete „Nichts-Namen“:
..* 'NaN'
..* 'undefined'
..* 'null'

###Operationen/ Operatoren

Arithmetische Operatoren

'+' (addieren, stringverkettung)
'-' (subtrahieren)
'*' (multiplizieren)
'/' (dividieren)
'%' (modulo)
'++' (inkrement)
'--' (dekrement)

Vergleichs Operatoren

'==' (wenn beiden gleich)
'!=' (wenn beide ungleich)
'<' (kleiner als)
'>' (grösser als)
'<=' (kleiner und gleich als)
'>=' (grösser und gleich als)
'==='(abfrage auf gleichen Datentypen)

Zuweisungs Operator

'=' (gleichheitszeichen)

###Kontrollstrukturen

Entscheidungsfindung

Das Skript entscheidet welchen Weg er gehen wird. If und Else ist also eine Abzweigung.
```javascript
var a = 5;
if(a < 6){
	
} else {
	
}

```
wenn(das in der klammer stimmt){
	dann mach das
} anderes(wenn es etwas anderes ist){
	dann mach das
}

Schleifen

Mit schleifen wiederholt man Anweisungen die in den geschweiften Klammern stehen. In den runden Klammen bestimmen wir wie lange der durch sein sollte. Es gibt 3 Arten von Schleifen:

..* For-Schleife
..* While-Schleife
..* Do-While-Schleife

```javascript
for (i = 0; i < 10; i++) {
	
}
```

