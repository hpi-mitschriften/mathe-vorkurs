# Aussageformen
Eine Aussageform ist ein sprachliches Gebilde, das mindestens eine [Variable](../Grundlagen/Variablen.md) enthält und nach geeigneter Ersetzung in eine (wahre oder falsche) [Aussage](./Aussagen.md) übergeht. Eine solche Ersetzung wird Belegung der Variablen genannt.

bsp.: $3+x = 5$
Werden erst dann zu [Aussagen](./Aussagen.md) wenn die vorkommenden [Variablen](../Grundlagen/Variablen.md) mit (zulässigen) Werten belegt werden. Dazu gehört ein **zulässiger Grundbereich** der Vorgegeben werden muss (z.B. x∈N).

Wie [Aussagen](./Aussagen.md) kann man Aussageformen miteinander Verknüpfen ([Aussageverknüpfungen](./Aussageverkn%C3%BCpfungen.md)) und man erhält neue Aussageformen.

## Quantoren
Außer der Belegung der [Variablen](../Grundlagen/Variablen.md) mit Werten gibt es noch andere Möglichkeiten aus einer [Aussageform](./Aussageformen.md) eine [Aussage](./Aussagen.md) zu machen. (Ein Grundbereich *M* muss vorgegeben sein.)
"Für alle $x$ (aus $M$) gilt $A(x)$"
"Für alle $x\in \mathbb{N}$ gilt $3+x=5$" -> falsche Aussage

Allquantor  Symbole: $∀$, $⋀$ #TODO(Beschreibung)
Existensquantor Symbole: $∃$, $⋁$ "Es existiert mindestens ein $x$ (aus $M$) mit $A(x)$"

$(∃x\in \mathbb{N}) (3 + x = 1)$ *falsch*
$(∃x\in \mathbb{N}) (3 + x = 1)$ *true*

"Es existiert höchstens ein $x$ mit $A(x)$"
$(∀x)(∀y) (A(x) ∧ A(y) => x < y)$ #TODO(=> ersetzen)

"Es gibt höchstens ein $x$ mit $A(x)$"
$((∃\lnot x) A(x) == ((∃x) A(x)) ∧ ((∀x) (∀y) A(x) ∧ A(y) => x = y$ #TODO(Formatting)

## Übung
1. Verdächtige: Achim (A), Bertram (B), Christin (C)
2. Der/Die Täter sind in der Gruppe der Verdächtigen zu finden
3. Wenn A und B nicht beide Beteiligt waren, dann hat C auch nicht mitgemacht.
4. Wenn B schuldig ist oder wenn C unschuldig ist kann A nicht der Täter sein

A|B|C|möglich
---|---|---|---
W|W|W|2, 3
W|W|F|3
W|F|W|2
F|W|W|2
F|W|F|wahr
F|F|F|1
$(A ∧ B ∧ C) ∧ (\lnot(A ∧ B) => \lnot C) ∧ ((B ∧ ¬C) => \lnot A)$
Ergebnis:  $¬A, B, \lnot C$