# CSS Basics

CSS steht für Cascading Style Sheets und wird verwendet, um das Aussehen von HTML-Elementen auf einer Webseite zu definieren. Hier sind die Grundlagen von CSS:

## Selektoren

CSS-Selektoren werden verwendet, um zu definieren, welche HTML-Elemente gestylt werden sollen. Selektoren können basierend auf Klassen, IDs, Attributen und mehr ausgewählt werden. Hier sind einige Beispiele:

- `#id-name`: Wählt ein Element mit einer bestimmten ID aus.
- `.class-name`: Wählt ein Element mit einer bestimmten Klasse aus.
- `element`: Wählt alle Elemente eines bestimmten Typs aus (z.B. `p`, `h1`, `div`).
- `element, element`: Wählt mehrere Elemente aus.
- `element > element`: Wählt Elemente aus, die ein anderes Element direkt enthalten. Beispiel `div > p`: 
```html
<div>
  <p>Ich werde ausgewählt</p>
  <a href="#">
    <p>Ich werde nicht ausgewählt</p>
  <a>
</div>
```

- `element element`: Wählt Elemente aus, die ein anderes Element enthalten (direkte Kinder und tiefer verschachtelt), Beispiel `div p`:
```html
<div>
  <p>Ich werde ausgewählt</p>
  <a href="#">
    <p>Ich werde auch ausgewählt</p>
  <a>
</div>
```
### Spezifität
Jeder Selektor hat eine eigene pezifität. Nur Selektoren mit gleicher oder höherer Spezifität können andere Selektoren überschreiben.
- Elementselektor --> 1
- Klassenselektor --> 10
- ID-Selektor --> 100

Bei kombinierte Selektoren wird die jeweilige Spzifität addiert, Beispiel:
`ul > .listItem` --> Spezifität 11 --> p (1) + .listItem(10)

## Eigenschaften

CSS-Eigenschaften definieren das Aussehen eines Elements, wie z.B. Farbe, Schriftart, Größe und Position. Hier sind einige grundlegende CSS-Eigenschaften:

### Farben
- `color`: Definiert die Schriftfarbe.
- `background-color`: Definiert die Hintergrundfarbe.

### Hintergrund
- `background-image`: legt Hintergrundbild fest, z.B. `background-image: url("meinBild.jpg") `
- `background-repeat`: Hintergrundbild soll sich wiederholen oder nicht
- `background-size` : Die Größe des Hintergrundbildes festlegen

### Text
- `font-family`: Definiert die Schriftart.
- `font-size`: Definiert die Schriftgröße.
- `font-style`: kursiv usw.
- `font-weight`: Schrift dünner/dicker
- `text-align`: Definiert die Textausrichtung.
- `text-decoration`: Text durchstreichen, unterstreichen

### Rahmen
- `border`: Definiert die Grenze des Elements - hat 3 Eigenschaften (dicke, Form, Farbe) z.B. `border: 1px solid black;`

### Abstände
- `margin`: Definiert den Außenabstand des Elements.
- `padding`: Definiert den Innenabstand des Elements.


## Einbindung von CSS

CSS kann auf eine Webseite auf verschiedene Arten eingebunden werden, z.B. durch Verlinkung einer externen CSS-Datei oder durch Einbetten von CSS direkt in die HTML-Datei:

### Externe CSS-Datei - *external*

Erstellen Sie eine separate CSS-Datei mit Ihren Stilen und verlinken Sie sie in Ihrer HTML-Datei, die Verlinkung erfolgt im `<head>`:

```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

### Einbetten von CSS in HTML - *internal*

Verwenden Sie das `<style>`-Tag, um CSS direkt in Ihre HTML-Datei einzubetten, auch das erfolgt im `<head>` Bereich:

```
<head>
  <style>
    h1 {
      color: red;
      font-size: 24px;
    }
  </style>
</head>
```

### CSS direkt in HTML Element einbetten - *inline*

Sie können ein HTML-Element mit einem `style`-Attriut versehen und so das Styling direkt verändern:
```html
<p style="color:green;">Ich bin ein grüner Text</p>
```

## Beispiele

Hier ist ein Beispiel für CSS-Stile, die auf HTML-Elemente angewendet werden:

```
/* Selektor für alle h1-Elemente */
h1 {
  color: blue;
  font-size: 36px;
}

/* Selektor für das Element mit der ID "meine-id" */
#meine-id {
  background-color: yellow;
}

/* Selektor für alle Elemente mit der Klasse "meine-klasse" */
.meine-klasse {
  border: 1px solid black;
}

/* Selektor für alle <a>-Elemente in <nav>-Elementen */
nav a {
  text-decoration: none;
}
```

## Ressourcen
Nachfolgend ein paar nützliche Ressourcen mit Links, geordnet zu den obigen Themen:
- [CSS Selektoren](https://kulturbanause.de/blog/css-selektoren/)
- [Übersicht verschiedene CSS-Eigenschaften](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften)
- [CSS Einbinden](https://wiki.selfhtml.org/wiki/CSS/Tutorials/Einstieg/Stylesheets_einbinden#direkt_in_einem_style-Attribut)
- [W3Schools als wichtige Referenz](https://www.w3schools.com/cssref/index.php)

<br><br>
[**--> zurück zur Übersicht**](/README.md)
