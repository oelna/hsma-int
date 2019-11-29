# HTML

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

## Stunde 2: Elemente

### Textabschnitte `<p>`, Betonung mit `<em>` und `<strong>`
```html
<p>fhsdj fhdjs hfdsjfh<br />dsjkf hsdjf hdjks fhdsjkf hdsjkf hdskjf</p>
<p>fhsdj fhdjs hfdsjfh dsjkf <em>hsfdfds dfs djf</em> hdjks fhdsjkf hdsjkf hdskjf</p>
<p>fhsdj fhdjs <strong>hfdsjfh</strong> fdj fdsjkf hsdjf hdjks fhdsjkf hdsjkf hdskjf</p>
```

### Listen `<ul>`, `<ol>`, `<li>`
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

### Zeitangaben mit `<time>`

```html
<p>
	<time datetime="2019-06-18">letzten Dienstag</time>
	<time datetime="2019-06-20 11:00:00">gestern morgen</time>
	<time datetime="2019-06-18">18. Juni 19</time>
</p>
```

## Stunde 3: Tabellen und Bilder

### Bilder `<img>`

```html
<img src="mein-bild.jpg" alt="Ein tolles Foto von mir" width="300" height="480" />

<img src="unterordner/mein-bild.jpg" alt="Ein tolles Foto von mir" />

<img src="bilder/lowres/mein-bild.jpg" alt="Ein tolles Foto von mir" />
```

### Tabellen `<table>`, `<tr>`, `<td>`, `<th>`

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

Der Klassenname wird mit einem Punkt `.` markiert.

```css
.aktiv {
	background-color: yellow;
}
```

### ID

Die ID wird mit einem Hash `#` markiert.

```css
#navigation {
	font-size: 13px;
}
```

### Elemente IN anderen Elementen

Alle `<time>`-Elemente in `<p>`-Elementen werden mit Schriftfarbe Rot formatiert.

```css
p time {
	color: red;
}
```

Alle `<img>`-Elemente in `<a>`-Elementen in Elementen mit der Klasse `.navigation` werden als Breite `200px` formatiert.

```css
.navigation a img {
	width: 200px;
}
```

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
| list-style | Art, wie listenaufzählungspunkte angezeigt werden |

### Einheiten

`CSS` einheiten: `px`, `em`, `%`

## Flexbox

Elemente nebeneinander oder untereinander anordnen

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

## Dieses Semester nicht:

- `position: absolute`
- `float`
