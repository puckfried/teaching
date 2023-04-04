# Grundlagen von JavaScript

JavaScript ist eine der wichtigsten Programmiersprachen für die Webentwicklung. Hier sind die Grundlagen von JavaScript:

## Variablen

In JavaScript können wir Variablen mit dem `let`-Schlüsselwort deklarieren. Eine Variable ist ein Container für Werte, die sich ändern können. Hier sind einige Beispiele:

```javascript
let name = "Max";
let alter = 25;
let istStudent = true;
```

## Datentypen

JavaScript hat mehrere Datentypen, einschließlich Strings, Zahlen, Booleans, Objekte und mehr. Hier sind einige Beispiele:
```javascript
let name = "Max"; // String
let alter = 25; // Zahl
let istStudent = true; // Boolean
let person = { name: "Max", alter: 25, istStudent: true }; // Objekt
```

## Operatoren
JavaScript hat verschiedene Arten von Operatoren, einschließlich mathematischer, Vergleichs- und logischer Operatoren. Hier sind einige Beispiele:
```javascript
let x = 10;
let y = 5;
let summe = x + y; // Addition
let differenz = x - y; // Subtraktion
let produkt = x * y; // Multiplikation
let quotient = x / y; // Division
let gleich = x === y; // Gleichheitsoperator
let ungleich = x !== y; // Ungleichheitsoperator
let und = x < 20 && y > 0; // Logisches und
let oder = x < 20 || y > 0; // Logisches oder
```


## Bedingungen
In JavaScript können wir Bedingungen mit if-Anweisungen definieren. Wenn eine Bedingung erfüllt ist, wird der Code innerhalb der Anweisung ausgeführt. Hier ist ein Beispiel:
```javascript
let alter = 18;
if (alter >= 18) {
  console.log("Du bist volljährig.");
} else {
  console.log("Du bist noch minderjährig.");
}
```

## Schleifen

In JavaScript können wir Schleifen verwenden, um eine Aktion mehrmals auszuführen. Hier ist ein Beispiel für eine for-Schleife:
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

## Javascript auf Webseite
Die Manipulation von DOM-Elementen ist ein wichtiger Teil der Webentwicklung. Entwickler können damit beispielsweise das Erscheinungsbild von Elementen ändern, Benutzerinteraktionen steuern oder Daten von Formularen sammeln und verarbeiten.

Die grundlegenden Schritte zur Manipulation von DOM-Elementen sind wie folgt:

- Zugriff auf das Element: Mit JavaScript kann auf DOM-Elemente zugegriffen werden, indem das entsprechende Element mit Hilfe von Selektoren ausgewählt wird.

- Änderung der Eigenschaften: Nachdem ein Element ausgewählt wurde, können mit JavaScript seine Eigenschaften geändert werden. Beispielsweise kann die Farbe, Größe oder Position eines Elements geändert werden.

- Hinzufügen oder Entfernen von Elementen: JavaScript ermöglicht es Entwicklern, neue Elemente in das DOM einzufügen oder vorhandene Elemente zu entfernen. Dadurch können beispielsweise neue Inhalte hinzugefügt oder Teile einer Webseite aktualisiert werden.

Mit der Manipulation von DOM-Elementen können Entwickler die Benutzererfahrung auf einer Webseite verbessern und dynamische Funktionalitäten hinzufügen. Mit JavaScript kann fast alles auf einer Webseite interaktiv und ansprechend gemacht werden.

### `document.querySelector` 
Die Methode querySelector wird verwendet, um das erste Element in einem HTML-Dokument auszuwählen, das mit einem gegebenen CSS-Selektor übereinstimmt. Das zurückgegebene Element ist ein Objekt, das viele Eigenschaften und Methoden hat, die verwendet werden können, um das Element zu manipulieren.

```javascript
// Wählt das erste Element mit der ID "meinElement" aus
const element = document.querySelector("#meinElement");

// Ändert den Text des Elements
element.textContent = "Hallo Welt!";
```

### `element.classList`

Die Eigenschaft classList eines Elements gibt eine Liste der Klassen zurück, die dem Element zugeordnet sind. Diese Liste kann durch verschiedene Methoden wie add, remove und toggle geändert werden, um die Klassen des Elements dynamisch zu ändern.

###### html:
```html
<div id="meinDiv" class="box"></div>
```
###### javascript
```javascript
// Wählt das Element mit der ID "meinDiv" aus
const element = document.querySelector("#meinDiv");

// Fügt eine neue Klasse "rot" hinzu
element.classList.add("rot");

// Entfernt die Klasse "box"
element.classList.remove("box");
```

### `element.style`
Die Eigenschaft style eines Elements ermöglicht es uns, die CSS-Eigenschaften des Elements direkt zu ändern. Jede CSS-Eigenschaft kann als Attribut aufgerufen und geändert werden.

###### html
```html
<div id="meinDiv"></div>
```

###### javascript
```javascript
// Wählt das Element mit der ID "meinDiv" aus
const element = document.querySelector("#meinDiv");

// Ändert die Hintergrundfarbe des Elements
element.style.backgroundColor = "rot";

// Ändert die Schriftgröße des Elements
element.style.fontSize = "24px";
```
