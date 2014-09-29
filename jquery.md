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

**Ready Document**

Man umklammert jede Funktion mit einem Ready Document. Weil jQuery erst bereit sein oder Zugriff gewähren sollte, wenn die Seite fertig geladen ist.
Diese geht wiefolgt so:

```js
$(document).ready(function(){

   // jQuery Methoden hier..

});
```

**Weitere Selektoren in jQuery**

| Syntax | Beschreibung |
| ------ | ------------ |
| $(" \* ") | Alle Elemente auswählen |
| $(this) | Ausgewähltes jetziges Element |
| $("p.intro") | Alle Paragraphen mit der Klasse 'Intro' |
| $("p:first") | Das erste Paragraphen Element |
| $("ul li:first-child") | Alle ersten `<li>` Elemente in jedem <ul> |
| $("a[target!='\ _ blank']") | Alle `<a>` Elemente die nicht gleich "\ _ blank" sind |

###Events

**Meist genutzten Events**

|Maus Events|Tastatur Events|Form Events|Document/ Window Events|
|---------|----------|----------|----------------|
|click|keypress|submit|load|
|dblclick|keydown|change|scroll|
|mouseenter|keyup|focus|resize|
|mouseleave|-|blur|unload|


##Ajax

Mit JavaScirpt, Daten vom Server nachgefordert werden, die dann mit DHTML in die Webseite eingebaut werden.
Dabei bleibt die bereits geladene Seite vorhanden. Hierfür braucht man eine implementierte Bibliotheke von jQuery.
Einbinden in die HTML-Datei:
```html
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.6.2/jquery.min.js" type="text/javascript">
</script>
```
