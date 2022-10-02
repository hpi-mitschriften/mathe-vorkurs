# Aussagevernüpfungen
Junktoren (Aussageverknüpfungen) sind Worte oder Zeichen, die Teilaussagen so zu einer Gesamtaussage verknüpfen, dass der Wahrheitswert der Gesamtaussage ausschließlich von den Wahrheitswerten der beteiligten Teilaussagen abhängt.

## Negation
*Negiert* die Aussagevariable. NOT-Gutter
#TODO(fig3)
A | ~A
---|---
F | *W*
W | *F*

## Konjunktion
Gibt an ob zwei Variablen den selben Wert haben.
#TODO(fig4)
A^B "A und B"
A | B | A^B
---|---|---
F | F | *W*
W | F | *F*
F | W | *F*
W | W | *W*

## Disjunktion
Gibt an ob bei zwei Aussagevariablen mindestens einmal der Wert *wahr* gegeben ist.
#TODO(fig5)
A | B | A+B #TODO(Zeichen ändern)
---|---|---
F | F | *F*
W | F | *W*
F | W | *W*
W | W | *W*

## Antivalenz
ausschließendes Oder (XOR)
#TODO(fig6)
A | B | A+B #TODO(Zeichen ändern)
---|---|---
F | F | *F*
W | F | *W*
F | W | *W*
W | W | *F*

## Implikation
Aus A folgt B #TODO(Text vervollständigen)
"Aus A folgt B", "Wenn A dann B", "A ist hinreichend für B", "B ist notwendig für A", "A impliziert B"
A -> Prämisse (Vorraussetzung)(hinreichende Bedingung)
B -> Konfusion (Konsequenz)(notwendige Bedingung)
A | B | A=>B #TODO(Zeichen ändern)
---|---|---
F | F | *W*
W | F | *W*
F | W | *F*
W | W | *W*

### Beispiel
Bei einem Kartenspiel sind auf der Vorderseite Buchstaben und auf der Rückseite Zahlen abgebildet.

Regel: *Wenn vorne ein Vokal steht, dann steht auf der Rückseite eine gerade Zahl.*

Welche der folgenden Karten müssen überprüft werden um den Wahrheitsgehalt der Aussage zu bestätigen.
\[A] \[B] \[1] \[2]

Antwort: *B und 1 sind für die Regel nicht relevant. A und 2 müssen überprüft werden um die Regel zu bestätigen.*

## Äquivalenz
#TODO(Text hinzufügen)
A <=> B 
- "B äquivalent mit A"
- "A genau dann, wenn B"

A | B | A<=>B
---|---|---
F | F | *W*
W | F | *F*
F | W | *F*
W | W | *W*
