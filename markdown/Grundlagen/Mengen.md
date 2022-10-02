# Mengen

"Unter einer Menge *M* verstehen wir eine Zusammenfassung von wohldefinierten Objekten *m* unserer Anschaung oder unseres Denkens, welche die Elemente von *M* genannt werden zu einem einheitlichen Ganzen" *Georg Cantor (1845 - 1918)*

## Schreibweise
- $m\in M$ ($m$ ist ein Element von $M$)
- $m \notin M$ ($m$ ist kein Element von $m$)
- für Mengen mit (wenigen) endlich vielen Elementen: $M \lbrace m, m², m³ \rbrace$
- allgemein mittels Eigenschaft $E(m)$ (Aussageform) $A = {m |E(m)}$ $A = {m \in M | E(m)} = {m | m \in M \land E (m)}$
	- $B' = {p\in N | 2 \geq p \land p \leq 12 \land p \in Primzahl}$
- leere Menge $\lbrace \rbrace$ $\emptyset = \lbrace x | x \neq x\rbrace$
- Einmenge $A = \lbrace a\rbrace$ oder $A = \lbrace x | x = a\rbrace$
- Zweimenge $A = \lbrace a, b \rbrace$ oder $A = \lbrace x | x = a \lor x = b\rbrace$
- $|A|$ oder $A$ Anzahl der Elemente in $A$ (wenn $A$ endlich)
- Andere: Natürliche Zahlen $\mathbb{N}$, Reele Zahlen $\mathbb{Z}$
- Teilmengen $A \subset B$,  $A$ ist Teilmenge von $B$, $B$ ist Obermenge von $A$. Ist $B$ eine Teilmenge von $C$ ist auch $A$ eine Teilmenge von $C$. Ist $A$ eine Teilmenge von $B$ und $B$ eine Teilmenge von $A$, gilt $A = B$. Wenn $B \nsubseteq A$ ist $A$ eine echte Teilmenge von $B$

## Problem
**Man darf nicht alle möglichen Zusammenfassungen bilden!**
Bsp.: Bernhard Russel $R = \lbrace M |$ M ist Menge $\land M \notin M \rbrace$
$R \in R <=> R \notin R$ (Wiederspruch) #TODO (<=> austauschen)

**Ausgang** Axiomatischer Aufbau der Mengenlehre. 

## Beispiel für ein Axiom
- **Existenzaxiom**: Zwei Mengen *A* und *B* sind genau dann gleich wenn sie dieselben Elemente haben. $A=B <=> (Vx)(x\in A <=> x\in B)$ #TODO (<=> austauschen)
	- $B = B'$
		- $\lbrace 1, 2, 3\rbrace == \lbrace2, 3, 1, 2, 3, 1\rbrace$ #TODO(== austauschen)