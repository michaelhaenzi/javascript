jQuery und Ajax
======

###Was ist jQuery?

jQuery ist eine JavaScript Bibliotheke. Sie beinhaltet:

* HTML/ DOM und CSS manipualtion
* HTML Event Methoden
* Effekte und Animationen
* Ajax
* Utilities
* *Plugins wenn benötigt*

###Warum jQuery?

jQuery hat sich durchgesetzt und ist derzeit einer der populärsten JavaScript Bibliotheken.
Jeder regulärer Browser unterstützt jQuery auch der Internet Explorer 6. jQuery wird zudem von Google und Microsoft unterstützt.

###Implementierung in eine Webseite

* Download der jQuery Bibliotheke
* Einfügen vom CDN (Content Delivery Network), wie z.B Google

**Download**

Es gibt 2 verfügbare Varianten um es sich zu Downloaden auf der jQuery Webseite:

* Die Produktions Version - diese ist verkleinert, für eine Live-Webseite
* Entwicklungs Version - nicht verkleinert, für Entwicklungs- und Testversuche.

Beide kann man auf [jQuery Webseite](http://jquery.com/download/) downloaden. Im Head der HTML-Datei gibt man den Pfad an mit `<script>`
```html
<head>
<script scr="jquery-1.11.1.min.js"></script>
</head>
```
**CDN**

Wieder gibt man die Bibliothek in den Head als `<script>` ein. Nur mit einem direkten Link zu Microsoft oder Google, welche die beiden Hosten.

Google:
```html
<head>
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
</head>
```

Microsoft:

```html
<head>
<script src="http://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.11.1.min.js"></script>
</head>
```

###jQuery Syntax

Die Grundsyntax von jQuery ist: `$(selector).action()`

* ein `$` Zeichen um jQuery anzukündigen
* ein `(selector)` um ein bestimmtes HTML-Element auszuwählen
* eine jQuery `action()` um eine Aktion durchzuführen.

Beispiele:

```js
$(this).hide()
 //verstecke dieses element (ausgewähltes).

$("p").hide()
 //verstecke alle Paragraphen.

$(".test").hide()
 //verstecke alle Elemente mit der Klasse 'test'.

$("#test").hide()
 //verstecke das Element mit der Id 'test'.
```
