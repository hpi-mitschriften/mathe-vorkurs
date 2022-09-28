# Aussagenlogische Terme
A| B| C || (($\lnot$ | A | $\land$|($\lnot$ | C))) | => | ((NOT | B) | $\land$ | A))
---|---|-|---|---|---|---|---|---|---|---|---|---|---
F | F | F || W | F | F | W | F | F | W | F | F | F
F | F | W || W | F | F | F | W | F | W | F | F | F
#TODO(Darstellung überarbeiten)

Zwei aussagenlogische Terme $W(A, B, C, ...)$ und $V(A , B, C, ... )$ heißen logisch äquivalent wenn sie den gleichen Wahrheitswertverlauf haben. ($W(A, B, C, ...) == V(A , B, C, ... )$).

Zwei Terme $W(A, B, C, ...)$ und $V(A , B, C, ...)$ sind genau dann logisch äquivalent, wenn der Term $W(A, B, C, ...) <=> *V(A , B, C, ... )$ eine Tautologie ist. #TODO(== und <=> ersetzen)

## Klammerregeln
- Außenklammern (um den ganzen [[Aussagenlogische Terme|Term]] #TODO(Terme definieren, Link überarbeiten)) können weggelassen werden
- Nach dem *Assoziativgesetz* können Klammern weggelassen werden wo sie nicht zu Bedeutung beitragen
- Nach dem *Kommutativgesetzt* können bei Operationen die keine logisch festgelegte Reihenfolge haben Variablen getauscht werden
- [[Aussageverknüpfungen#Negation|Negation]] bindet am stärksten: ($\lnot A \land B == (\lnot A) \land B$)
- [[Aussageverknüpfungen#Konjunktion|Konjunktionen]] binden am zweitstärksten ($A\land B+C == (A \land B) + G$)
- [[Aussageverknüpfungen#Disjunktion|Disjunktionen]] binden am drittstärksten 