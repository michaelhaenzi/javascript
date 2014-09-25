Video2Brain JavaScript
======================

###Wo kann ich diese Videos finden?

Hier ist ein explizieter JavaScript Crashkurs für Anfänger: [Video2Brain JavaScript](https://www.video2brain.com/de/videotraining/javascript-crashkurs-2012)

###Was ist JavaScript überhaupt?

Es dient der Aufbereitung von Daten über einen Server. JavaScript gestattet dynamische Aktionen auf einem Webserver. JS ist auf fast allen modernen und neueren Seiten aufzufinden.

###Wo wird JavaScript konkret eingesetzt?

* Dynamische Manipulation auf Webseiten (Document Object Model)
* Plausibilitätsprüfung (Prüfung eines Formulars)
* Senden, Empfangen von Daten (Ajax)
* Toolbar, dynamische Navigationsleisten und viele andere mehr…

Webseiten bei denen solche Funktionen genutzt werden:

* Google Map (Zoomen, Verschieben, Route berechnen etc.)
* Yahoo! (Formular Überprüfung)
* Andere Seiten

###Was braucht es um JavaScript anzuwenden?

Man sollte einige Grundkenntnisse von HTML und CSS haben. Denn ohne diesen 3er Bund wirkt es steif, langweilig und uninteressant.
Erforderliche Programme:
Man sollte einen IDE (integrated development environment) besitzen. Da gibt es einige sehr gute im Angebot, wie z.B.: Aptana Studio oder Visual Studio Web Developer.
Neben einem IDE sollte man verschiedene Browser gedownloadet haben. Da man Funktionalität auf den meist genutzten Browsern Test bevor man es öffentlich macht. Dabei eignet sich ganz gut: Firefox, Google Chrome, Internet Explorer, Opera und Safari.

###Firebug, was ist das?

„Firebug“ ist ein Addon was man im Firefox Browser sich gratis downloaden kann. Es hilft Entwicklern effektiv die Hintergründe der Webseite zu sehen und zu testen. Allgemein empfiehlt sich bei Firefox mit Firebug zu arbeiten.

###Wie fügt man nun ein JavaScript Skript in eine HTML-Seite ein?

Im Grunde ganz einfach, wie bei CSS. Es gibt 3 Arten beim Einbinden von JS. Durch eine Inline-Referenz, Skript-Container und Externe-Referenz. Diese 3 Arten werden hier ganz kurz erklärt:

| **Einbindungs-Art** | Beschreiung und Quellcode |
| ------------------------ | ------------------- |
| **Inline-Referenz** | Die JavaScript Funktion wird direkt in einem Inline-Element eingebunden. |
| Quellcode	| ```<a href="javascript:alert('Hallo')">Das ist eine Inline-Referenz</a> ``` |
| **Skript-Container** | Hierbei wird einem internen Block-Element eine JavaScript Anweisung zugeteilt. |
| Quellcode | ```<script> alert("Der interne Skript-Container"); </script> ``` |
| **Externe-Referenz** | Man integriert mit scr (source = quelle) eine externe .js Datei. Ist immer vorhanden |
| Quellcode | ```<script src="javascript.js"></script> ``` |


###Datentypen in JavaScript

Es gibt nur 4 Datentypen:
* **number** (Nummer: Ganze Zahlen und Kommazahlen)
* **string** (Text)
* **boolean** (True or False)
* **object** (Neues Objekt einfügen)

Diese Einteilung ist sehr weitläufig und daher auch sehr schlüpferig. Es gibt noch einen schöneren weg der Deklaration, das ist:
```js
var variabelnname = number, string, boolish oder object
```

Zudem ist 'var' (variable) eine nur interne Funktion.

###Undefined, not defined, null und NaN

Wenn man einem Variablennamen in js nichts zuteilt, also z.B.:
```js
var a;
```
dann ist 'a' definiert als 'undefined' welches eine eigene Funktionsnamen in JavaScript ist. Wenn man aber eine Variable ausgeben will ohne dass man sie vorher zugeteilt hat, dann gibt es einen Script-Fehler. Dann gibt es noch eine anderen Funktionsnamen ‚null‘ welcher bei der Kontrolle gibt. Wenn man versucht eine Operation von 2 Texten oder keinen Zahlen-Variablen ausgibt. Dann kommt ‚NaN‘ = ‚NotaNumber‘.

Im JavaScript verwendete „Nichts-Namen“:
* **NaN**
* **undefined**
* **null**

###Operationen/ Operatoren

**Arithmetische Operatoren**

\+ (addieren, stringverkettung)

\- (subtrahieren)

\* (multiplizieren)

/ (dividieren)

% (modulo)

\++ (inkrement)

\-- (dekrement)

**Vergleichs Operatoren**

== (wenn beiden gleich)

\!= (wenn beide ungleich)

< (kleiner als)

\> (grösser als)

<= (kleiner und gleich als)

\>= (grösser und gleich als)

=== (abfrage auf gleichen Datentypen)


**Zuweisungs Operator**

= (gleichheitszeichen)


###Kontrollstrukturen

**Entscheidungsfindung**

Man gibt hinter dem if und else einen Vergleichswert. Wenn es true (wahr) ist dann führt er das was in geschweiften Klammer ist aus.
```js
var a = 5;
if(a < 6){

} else {

}
```

**Schleifen**

Mit schleifen wiederholt man Anweisungen die in den geschweiften Klammern stehen. In den runden Klammen bestimmen wir wie lange der durch sein sollte. Es gibt 3 Arten von Schleifen:

* For-Schleife
* While-Schleife
* Do-While-Schleife

```js
for (i = 0; i < 10; i++) {

}
```
```js
while (i >= 10) {
	i++
}
```
```js
do {
	i++
}
while (i >= 10) {

}
```


**Sprunganweisung**

In bestimmten Situationen möchte man aus Schleifen früher raus. Also brauch man so genannte Sprunganweisungen:
* break; (bricht die Schleife ab)
* continue; (bricht den derzeitigen Durchlauf ab und geht mit dem nächsten Druchlauf weiter)
* return x; (liefert einen Rückgabe Wert)

###Funktion

**Funktionsaufbau**

Mit dem Keyword 'function' kündet man eine Funktion an. Einen aussagekräftigen Namen, und den Befehlen in den geschweiften Klammern, bilden das Gründgerüst für jede Funktion.
```js
function funktionsname() {
	alert("Hallo");
	alert("Welt");
}
```
In den runden Klammern gibt man die Parameter an, welche mit gegeben wurden. Um z.B. eine einfache Mathematik Aufgabe zu lösen:
```js
function multiplizieren(a, b) {
	alert(a*b);
}
```
**Lokale Variablen**

Lokale Variablen sind Variablen, die nur in dem sogenannten Gültigkeitsbereich einer Funktion verwendung finden.

**Aufruf einer Funktion**

Funktionen können mithilfe von HTML-Grundstrukturen in einer Webseite aufgerufen werden. Bedeutet: Man gibt einem Inline-/ Blockelement eine Funktion. Im obigen Beispiel haben wir Parameter mit a und b deklariert. Diese werden jetzt mit einem HTML-Link verküpft:
```html
<a href="javascript:multiplikation(2, 3)">Funktionsaufruf</a>
```
Wenn man jetzt auf den Link mit dem Namen "Funktionsaufruf" drauf klicken würde, würde die Funktion "multiplizieren" 2 * 3 rechnen. Es wurde einen alert("") auftauchen mit genau dem Resultat also 6.

**Eventhandler**

In jeden auf der Webseite, sichtbares Element kann man einen Eventhandler notieren.
 Ein Eventhandler ist ein Attribut unter HTML das ein Ereignis beschreibt.
 Z.B. den Klick mit der Maus:
```html
<button onclick="funktion(parameter)">
Buttonname
</button>
```
Eventhandler beginnen also mit "on" und beschreiben das Ereignis. Wenn der Mauszeiger über ein Bild gehen würde,
dann hiess der Eventhandler bei dem Bild "onmouseover". Würde er das Bilder wieder verlassen hiesse es "onmouseout".
Oder sogar den Klick bei einer Maus: "onmousedown" und "onmouseup". Man kann sich also die Attribute wunderbar merken.

**Rekursiver Aufruf**

Diese sind sogenannte Selbstaufrufe von Funktionen (Rekusive Aufrufe). Das heisst, in einer Funktion kann eine Funktion einer andere Aufrufen:
```js
function berechneFakultaet(){
	var a prompt("Geben sie eine Zahl ein");
	alert('Das Ergebnis von ' + a + '! lautet: ' + fakultaetRekursiv(a));
}
function fakultaetRekursiv(n) {
	if (n == 0) {
		return 1;
	} else {
		return n * fakultaetRekursiv(n - 1);
	}
}
```
Mit der Funktion "berechneFakultaet()" nehmen wir eine Zahl des Benutzers entgegen (prompt("")) welche wir mit der Variable a gespeichert haben.
Wir geben nun zuerst die eingegebne Zahl aus "a" und dann das Resultat der Funktion "fakultaetRekursiv(a)".
In dieser Funktion wird sie jetzt wieder aufgerufen um "n" bei jedem Druchlauf um eins zu vermindern. Sonst gäbe es ja eine Endlosschlaufe.
Diese Art der Funktionsaufruf wird häufig bei Animationen gebraucht.

###Objekte

**Was sind Objekte**

Ein Objekt ist ein Gegenstand der realen Welt, ein greifbarer Gegenstand den man beschreiben kann.
Ein Objekt hat demnach immer einen Befehl "Eigenschaften".
Zum Beispiel ein Papierkorb:

![Alt text](P:\GEOINFO\Hilfereiche Daten\GitHub\JavaScript\Video2Brain\Objekt1.png)

Die Methoden eines Objektes sind aktive Schritte welche man mit einem Objekt macht oder ein Objekt erledigt. Sie sind Funktionen die an ein Objekt gebunden sind.
Hier wieder das Beispiel:

![Alt text](P:\GEOINFO\Hilfereiche Daten\GitHub\JavaScript\Video2Brain\Objekt2.png)

Vorher war der Papierkorb noch voll und hatte ein Icon, bei dem man sieht das er gefüllt  ist.
Leert man ihn aber so wird das Icon und die Funktion "Papierkorb leeren" geändert. Die Funktion steht nichmeht zur Verfügung, weil der Zustand des Papierkorbes die Funktion nicht als sinnvoll erscheinen.

Fazit: Ein Objekt ist eine Sammlung von Eigenschaften und Methoden und die Methoden können abhängig von einem Zustand verfügbar sein, oder auch nicht.

**Wie erzeugt man jetzt ein neues Objekt?**

Dazu muss man wissen was eine Klasse in JavaScirpt ist: Eine Klasse ist eine Zusammenfassung von mehreren Objekten und Methoden.
Auch sogenannte "Bauvorschriften".
Hierbei gibt es eine Syntax die mit einem Schlüsselwort "new" beginnt.
Eine Standartklasse in JavaScirpt ist z.B. "Date". Also wird jetzt mithilfe
eines Konstruktors aus einer Klasse (z.B. "Date") ein Objekt.

```js
funktion objekteErzeugen(){
	var obj = new Date();
}
```
Es gibt noch eine Methode, ausser der Konstruktor-Methode, Objekte zu erzeugen.
Literal-Obejkte erzeugen:
```js
funktion objekteErzeugen(){
	var text = "Ich bin auch ein Objekt";
}
```
Also ist ein String (Zeichenkette) auch ein Objekt, da es auch eine Eigenschaft besitzt (Anzahl Zeichen).
Obwohl man in JavaScript als Liteale dies versteht:
```js
funktion objekteErzeugen(){
	var jsonobj = {
		"name":"Otto"
	};
}
```
Hierbei bildet man Wertepaare: Den Schlüssel ("name") und dem dazugehörigen Wert ("Otto").
Bei dieser Variante handelte es sich um Json (JavaScript Object Notation).

**Arrays**

Arrays und Objekte sind in JavaScript "so gut wie das gleich". Es ist eine Sammlung von Werten die über einen Bezeichner und ein Index zur verfügung gestellt.
In JavaScript sollte man Objekte als Arrays und Arrays als Objekte sehen.
Es gibt 3 Varianten einen Array zu erzeugen:

* Mithilfe der Konstruktor-Methode
* Json Notation
* Literale Form

```js
funktion arraysErzeugen(){
	var a1 = new Array();
	var a2 = {
		"name":"Meier",
		"vorname":"Otto"
	}
	var a3 = [1, 2, 3, 7, 9, 11];
}
```

**Dot and Array Notation**

Unter Dot Notation versteht man das Zugreifen auf ein/en Objekt oder Array.
Das geschiet - wie der name schon sagt - mit einem dot, also Punkt (.).
Sieht wie folgt aus:
```js
//Objekt
function objekteErzeugen(){
	var obj = new Date();
	alert(obj.getDay());
}
//Array 1
function arrayErzeugen1(){
	var a2 = {
		"name":"Meier",
		"vorname":"Otto"
	}
	alert(a2.vorname);
}
//Array 2
function arrayErzeugen2(){
	var a3 = [1, 2, 3, 7, 9, 11];
	alert(a3[2]);
}
```
Bei der ersten Funktion kommt der Wochentag in eine Zahl an z.B. Donnerstag = 4.
Bei der zweiten Funktion frage ich nach dem Wert von "vorname" also erscheint "Otto".
Bei der dritten Funktion wird 3 asugegeben, weil der Index [] mit 0 beginnt zu zählen.
Man greift in der Regel bei Objekten über die Dot Notation und bei den Arrays über die Array Notation.

**Klassenelemente**

Wenn man mehrere Objekte mit gleichen Klassen hat, muss man keinen Konstruktor dafür benutzen.
Man kann sie direkt in eine Funktion integrieren. Klassenelemente sind auch sogannte Konstanten. Da ihren Wert
z.B. bei Pi, Logarythmus 10 usw., in den nächsten Jahren nicht verändert wird:
```js
function klassenElemente(){
	Math.PI();
	Math.random();
}
```

###DOM-Konzept

**Was ist das DOM-Konzept?**

DOM (Document Objekt Model) ist ein Baumartigestruktur, mit Verzweigungen von Ästen (Knoten, engl. nodes) zu verstehen
Es ist also eine spezifikation für eine Schnittstelle um einen Zugriff auf HTML-Dokumente zu gewehrleisten.
Das DOM-Konzept finden sie auch bei FireBug.

**DOM-Objekte**

* **window** (Anzeigefenster, 'alert', 'confirm')
* **frame** (Frame-Fenster)
* **document** (Dokument im Anzeigefenster)
* **node** (Alle Knoten des Elementenbaums)
* **style** (CSS-Attribute von HTML-Elementen)
* **form** (Formulare  im Dokument)
* **element** (Formularelemente eines Formulars)
* **option** (Optionen einer Auswahlliste eines Formulars)
* **image** (Grafikreferenzen im Dokument)
* **event** (Anwenderereignisse)
* **history** (besuchte Seiten)
* **location** (URLs)
* **navigator** (Browser-Informationen)
* **screen** (Bildschrim-Informationen)

**Zugriffsmöglichkeiten auf DOM-Elemente**

Es gibt hauptsächlich zwei wichtige Zurgriffsmöglichkeiten auf Webseiten:

```js
function zugriff1() {
	//befehl(Dom-Objekt.Zugriffsbefehl("Tag")[Index].Eigenschaft)

	alert(document.getElementsByTagName("img")[0].src)
}
function zugriff2() {
	//befehl(Dom-Objekt.Zugriffsbefehl("Id").Eigenschaft)

	alert(document.getElementById("bild1").src)
}
```
Es gibt noch viele weitere Möglichkeiten auf Elemente zu zugreifen, die meisten sind aber veraltet und funktionieren nicht bei manchen Elementen.
Die 2 wichtigsten Zugriffsmöglichkeiten sind also über:
* **getElementsByTagName**
* **getElementById**

**Wichtigsten Aktionen der DOM-Elementen**

Im HTML-Dokument:
```html
<img src="images/b1.jpg" alt="Aus der Luft" name="bild1" id="b1" onmouseover="groesser()" onclick="infoBild1()"/>
```
Im JavaScript-Dokument:
```js
function groesser() {
	document.getElementById("b1").width += 20;
}
function infoBild1() {
	document.getElementById("bild1info").innerHTML = document.getElementById("b1").height;
}
```
