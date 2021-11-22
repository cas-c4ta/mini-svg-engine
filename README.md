# Mini SVG-Engine

Der Versuch, Chrigis komplexe SVG-Engine aufs Minimum herunterzubrechen.

Die Engine ist kein Objekt mit Methoden, sondern besteht nur aus ein paar Funktionen.

## theSVG

Die Variable, die das SVG-Element enthält

## newCircle(x, y, rad, col)

Funktion, die ein `<circle>`-Element generiert und dem SVG-Element als Kind anhängt.

Braucht als Argument x- und y-Positionen, einen Radius und eine Farbe.

Die Funktion gibt das neue `<circle>`-Element auch zurück, so dass es in eine Variable gespeichert werden kann:

```
let myNewCircle = newCircle(7, 5, 4, "crimson")
someArray.push(myNewCircle)
```

## getCirclePos(targetCircle)

Gibt die Positionsdaten eines `<circle>`-Elements zurück.

```
let pos = getCirclePos(myNewCircle)
console.log(pos) // {x: 7, y: 5}
```

## updateCirclePos(targetCircle, newX, newY)

Überschreibt die Positionsdaten eines `<circle>`-Elements.

```
updateCirclePos(myNewCircle, 6, 6)
let pos = getCirclePos(myNewCircle)
console.log(pos) // {x: 6, y: 6}
```
