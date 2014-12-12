Video2Brain JavaScript
======================


###Was ist JavaScript überhaupt?

JavaScript ist eine Programmiersprache die häufig im Clientbereich, das heisst beim Benutzer einer Website oder Webapp eingesetzt wird. JavaScript wird aber immer öfter auch als Backendsprache verwendet.
Es dient der Aufbereitung von Daten über einen Server. JavaScript gestattet dynamische Aktionen auf einer Webseite.

###Wo wird JavaScript konkret eingesetzt?

* Dynamische Manipulation auf Webseiten (Document Object Model)
* Plausibilitätsprüfung (Prüfung eines Formulars)
* Senden, Empfangen von Daten (Ajax)
* Toolbar, dynamische Navigationsleisten und viele andere mehr…

Webseiten bei denen solche Funktionen genutzt werden:

* Google Map (Zoomen, Verschieben, Route berechnen etc.)
* Yahoo! (Formular Überprüfung)
* Amazon (Wahrenkorb, Einkäufe)
* Weitere Seiten

###Was braucht es um JavaScript anzuwenden?

Um JavaScript anzuwenden sollte man sich bereits mit HTML und CSS auskennen. Denn JavaScript wird dazu verwendet eine Website dynamisch zu gestalten. Man kann bereits mit HTML und CSS eine sehr gute Website realisieren, für richtig komplexe Funbktionalitäten kommt man aber nicht um JavaScript herum.
Erforderliche Programme:
Zum Erstellen einer einfachen Website genügt ein Editor wie Sublime oder Atom. Doch auch Visual Studio oder Aptana Studio sind dafür geeignet. Natürlich will man seine Websites auch auf Aussehen und Funktionalität testen können und sollte daher einen oder mehrere Browser installiert haben.

**Firebug, was ist das?**

Firebug ist ein Addon für den Firefox Browser. Es ist ein Tool welches erlaubt die Console zu lesen und den Quellcode der Website einzusehen. Man sollte es sicherlich installieren wenn man diesen Browser bevorzugt.

###Wie fügt man nun ein JavaScript Skript in eine HTML-Seite ein?

Es gibt 3 Arten beim Einbinden von JS. Durch eine Inline-Referenz, Skript-Container und Externe-Referenz. Diese 3 Arten werden hier ganz kurz erklärt:

| **Einbindungs-Art** | Beschreiung und Quellcode |
| ------------------------ | ------------------- |
| **Inline-Referenz** | Die JavaScript Funktion wird direkt in einem Inline-Element eingebunden. |
| Quellcode	| ```<a href="javascript:alert('Hallo')">Das ist eine Inline-Referenz</a> ``` |
| **Skript-Container** | Hierbei wird einem internen Block-Element eine JavaScript Anweisung zugeteilt. |
| Quellcode | ```<script> alert("Der interne Skript-Container"); </script> ``` |
| **Externe-Referenz** | Man integriert mit scr (source = quelle) eine externe .js Datei. Ist immer vorhanden |
| Quellcode | ```<script src="javascript.js"></script> ``` |


###Die Variable '`var`'

Man benutzt für eine neue Variable einfach das Schlüsselwort `var`. Dieses  Schlüsselwort kann folgende "Wertarten" haben:

* **number** (Nummer: Ganze Zahlen und Kommazahlen)
* **string** (Text)
* **boolean** (True or False)
* **object** (Neues Objekt einfügen)

Eine einfache Deklaration in JavaScript:
```js
var zahl = 7,
	text = "Hallo Welt",
	bool = true;
var objekt = {
		vorname: 'Peter',
		nachname: 'Meier'
}
```

**Undefined, not defined, null und NaN**

Wenn man versucht eine Operation mit keiner Zahl Variablen auszugeben, dann kommt 'NaN', was ausgeschrieben 'NotaNumber' bedeutet.
Wenn man einer Variable in JavaScirpt keinen wert zuteilt, also z.B.: `var a;`, dann ist die Variable `a`  nicht definiert 'undefined'. Welches einen eigenen Funktionsnamen in JavaScript darstellt.
Da gibt es noch 'null' und 'null' bedeutet leer.
Keines dieser 3 sind in dem Sinne "Nichts" weil JavaScript NaN, undefined und null defierniert hat.

* NaN
* undefined
* null

###Operatoren

**Arithmetische Operatoren**

\+ (addieren, Stringverkettung)

\- (subtrahieren)

\* (multiplizieren)

/ (dividieren)

% (Modulo)

\++ (Inkrement)

\-- (Dekrement)


**Vergleichs Operatoren**

== (gleich)

\!= (ungleich)

< (kleiner als)

\> (grösser als)

<= (kleiner oder gleich als)

\>= (grösser oder gleich als)

=== (Abfrage auf gleichen Wert und Art des Wertes)


**Zuweisungs Operator**

= (Gleichheitszeichen)

**Verknüpfungs-Operatoren**
* && (UND-Verknüpfung)
* || (ODER-Verknüpfung)
* />> (Bitverschiebung rechts)
* << (Bitverschiebung links)

###Kontrollstrukturen

**Entscheidungsfindung**

Man gibt in den Klammern nach dem if eine Bedingung an die geprüft werden soll. Ist diese true (wahr) so wird der `Block A` ausgeführt, ist sie false (unwahr) so wird der `Block B` ausgeführt.
```js
var a = 5;
if(a < 6){
			//Block A
} else {
			//Block B
}
```

**Schleifen**

Mit Schleifen hat man die Möglichkeit Anweisungsblöcke zu wiederholen, diese Blöcke werden in geschweiften Klammern definiert. In den runden Klammern steht die Bedingung zu welcher dieser Block ausgeführt werden kann. Es gibt 3 Arten von Schleifen:

* For-Schleife
* While-Schleife
* Do-While-Schleife

```js
for (i = 0; i < 10; i++) {
	// Diese Schleife startet bei i=0,
	// sie führt den Block einmal aus und erhöht i um eins (i++)
	// Dies wird so oft getan, bis i nicht mehr kleiner ist als 10 (i < 10)
}


while (i >= 10) {
	i++;
	// Diese Schleife wird solange auzgeführt, wie i<=10 ist
}


do {
	i++;
	// Diese Schleife wird mindestens einmal ausgeführt,
	// danach wird die Bedingung geprüft, ist diese true (wahr),
	// so wird der Block erneut ausgeführt.
}
while (i >= 10)
```


**Sprunganweisung**

In bestimmten Situationen möchte man aus Schleifen früher raus. Daher brauch man so genannte Sprunganweisungen:
* break; (bricht die Schleife ab)
* continue; (bricht den derzeitigen Durchlauf ab und geht mit dem nächsten Druchlauf weiter)
* return x; (liefert einen Rückgabe Wert an die aufrufende Funktion. Somit wird die aktuelle Funktion beendet.)

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

Funktionen können mithilfe von HTML-Grundstrukturen in einer Webseite aufgerufen werden. Bedeutet: Man gibt einem Inline-/ Blockelement eine Funktion. Im Beispiel weiter oben haben wir Parameter mit a und b weitergegeben. Diese werden jetzt mit einem HTML-Link verküpft:
```html
<a href="javascript:multiplikation(2, 3)">Funktionsaufruf</a>
```
Wenn man jetzt auf den Link mit dem Namen "Funktionsaufruf" drauf klicken würde, würde die Funktion "multiplizieren" 2 * 3 rechnen. Es wurde einen alert("") auftauchen mit genau dem Resultat also 6.

**Eventhandler**

Auf jeder Webseite, kann man in einem sichtbarem Element einen Eventhandler notieren.
Ein Eventhandler ist ein Attribut unter HTML das ein Ereignis beschreibt.
Zum Beispiel den Klick mit der Maus:
```html
<button onclick="funktion(parameter)">
Buttonname
</button>
```
Eventhandler beginnen also mit "on" und beschreiben das Ereignis. Wenn der Mauszeiger über ein Bild gehen würde,
dann hiess der Eventhandler bei dem Bild "onmouseover". Würde der Cursor das Bilder wieder verlassen, so hiesse es "onmouseout".
Oder sogar den Klick bei einer Maus: "onmousedown" und "onmouseup". Man kann sich also die Attribute wunderbar merken.

**Rekursiver Aufruf**

Diese sind sogenannte Selbstaufrufe von Funktionen (Rekusive Aufrufe). Das heisst also, dass in einer Funktion die gleiche Funktion aufgeruft werden kann:
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
Mit der Funktion "berechneFakultaet()" nehmen wir eine Zahl des Clients entgegen - `prompt(" ")` - welche wir mit der Variable `a` gespeichert haben.
Wir geben nun zuerst die eingegebne Zahl `a` aus und dann das Resultat der Funktion `fakultaetRekursiv(n)`.
In dieser Funktion wird sie jetzt wieder aufgerufen um `n` bei jedem Druchlauf um eins zu vermindern. Sonst gäbe es ja eine Endlosschlaufe.
Diese Art der Funktionsaufruf wird häufig bei Animationen gebraucht.

###Objekte

**Was sind Objekte**

Ein Objekt ist ein Gegenstand der realen Welt, ein greifbarer Gegenstand den man beschreiben kann.
Ein Objekte hat demnach immer "Eigenschaften".
Beispiel am Papierkorb:

![Alt text](https://github.com/michaelhaenzi/javascript/blob/master/Objekt1.PNG)

Die Methoden eines Objektes sind aktive Schritte welche man mit einem Objekt macht oder ein Objekt erledigt. Sie sind Funktionen die an ein Objekt gebunden sind.
Hier wieder das Beispiel:

![Alt text](https://github.com/michaelhaenzi/javascript/blob/master/Objekt2.PNG)

Vorher war der Papierkorb noch voll und hatte ein Icon, bei dem man sieht das er gefüllt ist.
Leert man ihn aber so wird die Funktion "Papierkorb leeren" aufgerufen, welche die darin liegenden Dateien endgültig löscht und das Icon ändert. Die Funktion steht nichmehr zur Verfügung, weil der Zustand (eine Propertie) des Papierkorbes leer ist und es somit keinen Sinn macht diese Funktion auszuführen.

*Fazit: Ein Objekt ist eine Sammlung von Eigenschaften und Methoden und die Methoden können abhängig von einem Zustand verfügbar sein, müssen aber nicht.*

**Wie erzeugt man jetzt ein neues Objekt?**

Dazu muss man wissen was eine Klasse ist: Eine Klasse ist eine Zusammenfassung von mehreren Objekten und Methoden.
Hierbei gibt es eine Syntax die mit einem Schlüsselwort `new` beginnt.
Eine Standartklasse in JavaScirpt ist z.B. `Date`. Also wird jetzt mithilfe
eines Konstruktors aus einer Klasse (z.B. 'Date') ein Objekt (eine Instanz dieser Klasse) erzeugt.
Man könnte sie auch mit einer "Bauvorschrift" vergleichen.

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
Hierbei bildet man Wertepaare: Den Schlüssel (`name`) und dem dazugehörigen Wert (`Otto`).
Bei dieser Variante handelte es sich um Json (JavaScript Object Notation).

**Arrays**

Arrays und Objekte sind in JavaScript "so gut wie das gleiche". Es ist eine Sammlung von Werten die über einen Bezeichner und ein Index zur verfügung gestellt werden.
In JavaScript sollte man Objekte als Arrays und Arrays als Objekte sehen.
Es gibt 3 Varianten einen Array zu erzeugen:

* Mithilfe der Konstruktor-Methode (`var a1`)
* Json Notation (`var a2`)
* Literale Form (`var a3`)

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
Das geschiet - wie der name schon sagt - mit einem dot, also Punkt (`.`).
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
Bei der zweiten Funktion frage ich nach dem Wert von `vorname` also erscheint `Otto`.
Bei der dritten Funktion wird 3 ausgegeben, weil der Index `[ ]` mit 0 beginnt zu zählen.
Man greift in der Regel bei Objekten über die Dot Notation und bei den Arrays über die Array Notation.

**Klassenelemente**

Wenn man mehrere Objekte mit gleichen Klassen hat, muss man keinen Konstruktor dafür benutzen.
Man kann sie direkt in eine Funktion integrieren. Klassenelemente sind auch sogannte Konstanten. Da ihren Wert
z.B. wie bei Pi und Logarythmus 10, in den nächsten Jahren nicht verändert wird:
```js
function klassenElemente(){
	Math.PI();
	Math.random();
}
```

###DOM-Konzept

**Was ist das DOM-Konzept?**

DOM (Document Objekt Model) ist eine baumartige Struktur, mit Verzweigungen von "Ästen" (Knoten, engl. nodes) zu verstehen.
Es ist also eine spezifikation für eine Schnittstelle um einen Zugriff auf HTML-Dokumente zu gewehrleisten.


**DOM-Objekte**

* **window** (Anzeigefenster, `alert`, `confirm`)
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
Die zwei wichtigsten Zugriffsmöglichkeiten sind also über:

* `getElementsByTagName`
* `getElementById`

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
Wichtig ist hierbei das man mit .attribut fast alle Attribute von HTML anschreiben kann. Mit .innerHTML kann man  - wie der name schon sagt -  alle inneren Strukturen einer HTML-Datei löschen, ändern undneu bestimmen.
Das macht JavaScript so weitläufig und weiterführend.

**Funktionsreferenzen und anonyme Funktionen**

Statt Befehle direkt in ein HTML-Dokument einzubinden, verwendet man eine exterene JS-Datei.

```js
function init() {
	document.getElementById("b1").onmouseover = function() {
		document.getElementById("b1").width += 20;
	}
}
window.onload=init;
```
Das ist eine anonyme Funktion, weil sie keinen Funktions Namen hat. Doch ist sie ansprechbar durch die Id ihres Elementes.
Damit dieses DOM-Element überhaupt funktionieren, müssen sie erst nach dem laden der Seite aktiv werden.
Dafür gibt es einen Zeiger (`windows.onload=init;`).

**DHTML**

DHTML steht für 'Dynamic Hypertext Markup Language'.
DHTML grenzt an Animationen an, sie sind für kleinere "Animationen" gedacht. Wie etwa das vergrössern und verkleinern eines Textes. Man kann sie mit oder ohne JavaScript schreiben.

**Animationen**

Typisch für Animationen sind kleine, grosse oder sogar fazinierende Animationen. Hier wieder ein Beispiel dazu:
```js
function animation() {
	if (document.getElementsByTagName("img")[0].width++ < 300).setTimeout('animation()', '1');
}
window.onload = function() {
	document.getElementsByTagName("button")[0].onlick = animation;
}
```
Hierbei vergrössert sich das erste Bild mit dem Tag `img` immer um 1 Pixel bis zu maximal 300px. Hierbei ist dieses `.setTimeout` wichitg anzusehen.
Denn es macht nach jedem "Vergrössern", 1 Millisekunde Pause. Wir sehen diese Pausen nicht, daher erscheint das ganze flüssig.


<br />
*Quelle:
[Video2Brain, JavaScript Crashkurs](https://www.video2brain.com/de/videotraining/javascript-crashkurs-2012)*

<br />
```
Michael Haenzi, Switzerland 2014
```
