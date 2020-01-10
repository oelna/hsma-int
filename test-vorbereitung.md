# HTML

- Denke daran, auch immer die `.pdf`-Präsentationen der jeweiligen Stunde zu wiederholen!  
- Die Benutzung von Sublime Text für die Prüfung ist erlaubt
- Die Verwendung eigener, vorhandener HTML-Dateien ist verboten
- Die Online-Recherche, zB. über Google, etc. ist verboten

## Grundgerüst

```html
<!DOCTYPE html>
<html lang="de">
<head>
	<meta charset="utf-8" />
	<title>Meine Website</title>

	<link rel="stylesheet" href="website.css" />
</head>
<body>

</body>
</html>
```

## Stunde 1: Links

```html
<a href="andere_seite.html">Andere Unterseite auf meiner Seite</a>

<a href="http://www.google.com/">Andere Website</a>
```

Referenz: [MDN: a](https://developer.mozilla.org/de/docs/Web/HTML/Element/a)

## Stunde 2: Elemente

### Überschriften `<h1>`, `<h2>`,`<h3>` …

Beachte: Die Zahlen sind keine aufsteigende Nummerierung, sondern eine Gewichtung!
Meist braucht man nicht mehr als `<h1>`-`<h3>`, um seinen Inhalt sinnvoll zu gliedern.

```html
<h1>Süddeutsche Zeitung</h1>
<h2>Westen fordert von Iran Transparenz</h2>
<h2>240 000 Menschen sollen ihr Zuhause verlassen</h2>
<h2>Ein Chalet, ein Porsche, ein Streit</h2>
```

Referenz: [MDN: h1-h6](https://developer.mozilla.org/de/docs/Web/HTML/Element/h1-h6)

### Textabschnitte `<p>`, Betonung mit `<em>` und `<strong>`
```html
<p>fhsdj fhdjs hfdsjfh<br />dsjkf hsdjf hdjks fhdsjkf hdsjkf hdskjf</p>
<p>fhsdj fhdjs hfdsjfh dsjkf <em>hsfdfds dfs djf</em> hdjks fhdsjkf hdsjkf hdskjf</p>
<p>fhsdj fhdjs <strong>hfdsjfh</strong> fdj fdsjkf hsdjf hdjks fhdsjkf hdsjkf hdskjf</p>
```

Referenz: [MDN: p](https://developer.mozilla.org/de/docs/Web/HTML/Element/p), [em](https://developer.mozilla.org/de/docs/Web/HTML/Element/em), [strong](https://developer.mozilla.org/de/docs/Web/HTML/Element/strong)

### Listen `<ul>`, `<ol>`, `<li>`

Listen verwenden zwei verschiedene Tags, um die Struktur anzulegen; den Listencontainer und die Listeneinträge.

```html
<ul>
	<li>Punkt A</li>
	<li>Punkt B</li>
	<li>Punkt C</li>
</ul>

<ul>
	<li>
		<a href="seite_1.html">Punkt A</a>
	</li>
	<li>
		<a href="seite_2.html">Punkt B</a>
	</li>
	<li>
		<a href="seite_3.html">Punkt C</a>
	</li>
</ul>

<ol>
	<li>Lied 1</li>
	<li>Lied 2</li>
	<li>Lied 3</li>
</ol>
```

**Vorschau** `<ul>`:

- Punkt A
- Punkt B
- Punkt C

**Vorschau** `<ul>` mit Links:

- [Punkt A](https://developer.mozilla.org/de/docs/Web/HTML/Element/li)
- [Punkt B](https://developer.mozilla.org/de/docs/Web/HTML/Element/li)
- [Punkt C](https://developer.mozilla.org/de/docs/Web/HTML/Element/li)

**Vorschau** `<ol>`:

1. Punkt A
1. Punkt B
1. Punkt C

Referenz: [MDN: ul](https://developer.mozilla.org/de/docs/Web/HTML/Element/ul), [ol](https://developer.mozilla.org/de/docs/Web/HTML/Element/ol), [li](https://developer.mozilla.org/de/docs/Web/HTML/Element/li)

### Zeitangaben mit `<time>`

Maschinenlesbare Zeitangaben. Das `datetime`-Attribut akzeptiert u.a. ein Datum in der Form Jahr-Monat-Tag (`YYYY-MM-DD`) und/oder eine Zeitangabe in der Form Stunden:Minuten:Sekunden (`HH:MM:SS`).

```html
<p>
	<time datetime="2019-06-18">letzten Dienstag</time>
	<time datetime="2019-06-20 11:00:00">gestern morgen</time>
	<time datetime="2019-06-18">18. Juni 19</time>
</p>
```

Referenz: [MDN: time](https://developer.mozilla.org/de/docs/Web/HTML/Element/time)

## Stunde 3: Tabellen und Bilder

### Bilder `<img>`

Bilder haben immer ein "source"-Attribut `src`, um die zu ladende Bilddatei anzugeben (relative oder absolute URL). Die Datei kann in den Formaten `.jpg`, `.png`, `.gif` und `.svg` vorliegen und sollte im besten Fall eine Größe von ca. `50-150 kb` nicht überschreiten.  
Die Dimensionen des Bildes sollten im `<img>`-Element in den Attributen `width` (Breite) und `height` (Höhe) angegeben werden (Ohne Einheit, gemeint sind immer Pixel).  
Das `<img>`-Element sollte immer ein `alt`-Attribut haben, das in 1-2 kurzen Sätzen den Bildinhalt widergibt. Bei rein dekorativ verwendeten Bildern kann das Attribut einen leeren Wert haben ("").  

```html
<img src="mein-bild.jpg" alt="Ein tolles Foto von mir" width="300" height="480" />

<img src="unterordner/dateiname.jpg" alt="" />

<img src="bilder/lowres/mein-bild.jpg" alt="Ein tolles Foto von mir" />

<img src="http://www.tagesschau.de/multimedia/bilder/gruene282~_v-videowebl.jpg" alt="Die Geschichte der Grünen Partei" />
```

Referenz: [MDN: img](https://developer.mozilla.org/de/docs/Web/HTML/Element/img)

### Tabellen `<table>`, `<tr>`, `<td>`, `<th>`

Tabellen werden aus mindestens 3-4 verschiedenen Elementen zusammengesetzt, in der Reihenfolge 

1. Tabellencontainer [`<table>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/table)
1. Zeilen [`<tr>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/tr)
1. Inhaltszellen [`<td>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/td) oder Überschriftenzellen [`<th>`](https://developer.mozilla.org/de/docs/Web/HTML/Element/th)

Für die Konstruktion ist es manchmal einfacher, das veraltete Attribut `border` einzusetzen, um Gitternetzlinien angezeigt zu bekommen, da ansonsten die Rahmen der Tabelle unsichtbar sind (ausser man verwendet CSS, um sie einzublenden).

```html
<table border="1">
	<tr>
		<th>überschrift 1</th>
		<th>überschrift 2</th>
		<th>überschrift 3</th>
		<th>überschrift 4</th>
	</tr>
	<tr>
		<td class="bla">zelle 1</td>
		<td>zelle 2</td>
		<td>zelle 3</td>
		<td>zelle 4</td>
	</tr>
</table>
```

**Vorschau**

| überschrift 1 | überschrift 2 | überschrift 3 | überschrift 4 |
| --- | --- | --- | --- |
| zelle 1 | zelle 2 | zelle 3 | zelle 4 |

# CSS

## Stunde 4: Selektoren

Geschwungene Klammer geht am Mac mit `Alt/Option ⌥` + `(`, bzw. `Alt/Option ⌥` + `)`

```css
Selektor {
	Eigenschaft: Wert;
}
```

```css
p {
	font-size: 14px;
}
```

## Stunde 5: Klassen, ID, Verschachtelung

### Klassen

Das `class`-Attribut wird in HTML verwendet, um ein oder mehrere Elemente als einer benannten Gruppe zugehörig zu markieren.

```html
<p>Etwas <span class="markiert">wichtiger</span> Text.</p>
```

Das Element kann dann in CSS anhand seiner Klasse angesprochen werden. Der Klassenname wird dabei mit einem Punkt `.` markiert.

```css
.markiert {
	background-color: yellow;
}
```

Referenz: [MDN: class-Attribut](https://developer.mozilla.org/de/docs/Web/HTML/Globale_Attribute/class)

### ID

Das `id`-Attribut wird in HTML verwendet, um Elemente eindeutig zu benennen.

```html
<div id="navigation">…</div>
```

Das Element kann dann in CSS anhand seiner ID angesprochen werden. Die ID wird dabei mit einem Hash `#` markiert.

```css
#navigation {
	font-size: 13px;
}
```

Referenz: [MDN: id-Attribut](https://developer.mozilla.org/de/docs/Web/HTML/Globale_Attribute/id)

### Elemente IN anderen Elementen

Werden zwei Selektoren durch ein Leerzeichen verbunden, so wird das Element nur dann angesprochen, wenn es ein Nachfahrenelement eines anderen Elements ist. Dabei muss es kein direktes Kindelement sein, sondern kann auch weiter unten im Elementbaum notiert sein.

**Beispiel 1**

```html
<p>Wir waren <time>gestern</time> schwimmen.</p>
```

Alle `<time>`-Elemente in `<p>`-Elementen werden mit Schriftfarbe Rot formatiert.

```css
p time {
	color: red;
}
```

**Beispiel 2**

Alle `<img>`-Elemente in `<a>`-Elementen in Elementen mit der Klasse `.navigation` werden als Breite `200px` formatiert.

```css
.navigation a img {
	width: 200px;
}
```

Referenz: [MDN: Nachfahrenselektoren](https://developer.mozilla.org/en-US/docs/Web/CSS/Descendant_combinator), [Selfhtml: Nachfahrenkombinator](https://wiki.selfhtml.org/wiki/CSS/Selektoren/Kombinator/Nachfahrenkombinator)

## Im Test vorkommend:

### Eigenschaften

| Name | Bedeutung |
| --- | --- |
| color | Schriftfarbe |
| background | Hintergrundfarbe |
| background-color | Hintergrundfarbe |
| font-family | Schriftfamilie |
| font-size | Schriftgröße |
| line-height | Zeilenabstand |
| font-weight | Schriftgewicht |
| font-style | kursiv oder normal |
| text-decoration | unterstrichen, nicht unterstrichen |
| text-align | linksbündig, rechtsbündig, zentriert |
| border | Rahmenlinie für Elemente |
| margin | Aussenabstand |
| padding | Innenabstand |
| width | Breite des Elements |
| height | Höhe des Elements |
| list-style | Art, wie Listenaufzählungspunkte angezeigt werden |

### Einheiten

- `px`: Repräsentieren (unter Vorbehalt) einen Bildpunkt am Bildschirm in der jeweiligen Auflösung
- `em`: Ein `em` repräsentiert die vom Browser berechnete Schriftgröße des Elements
- `%`: Prozentangaben in einer Eigenschaft beziehen sich auf einen Bruchteil des verfügbaren Platzes

Nicht im Test aber interessant:

- `rem`
- `ex`
- `ch`
- `vw`
- `vh`
- `calc()`

Referenz: [SelfHTML: Maßeinheiten](https://wiki.selfhtml.org/wiki/CSS/Wertetypen/Zahlen,_Ma%C3%9Fe_und_Ma%C3%9Feinheiten)

## Flexbox

Elemente nebeneinander oder untereinander anordnen  
Im Test gefragt sind nur `display: flex` und die Eigenschaft `flex-direction`.

```html
<div class="test">
	<p>x</p>
	<p>y</p>
	<p>z</p>
</div>
```

```css
.test {
	display: flex;
	flex-direction: row;
}

/* oder */

.test {
	display: flex;
	flex-direction: column;
}
```

Referenz: [SelfHTML: Flexbox](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Flexbox)

## Dieses Semester nicht:

- `position: absolute`
- `float`
