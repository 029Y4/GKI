    # Lösung Übungsblatt: Problemlösen, Suche

## Bonus: Verlässlichkeit von ChatGPT (2P)

- **ToDo**

## Games.01: Handsimulation: Minimax und alpha-beta-Pruning (3P)

### 1. 


<picture><source media="(prefers-color-scheme: light)" srcset="images/alphabeta_light.png"><source media="(prefers-color-scheme: dark)" srcset="images/alphabeta_dark.png"><img src="images/alphabeta.png"></picture>


### 2. 

<br>


## Games.02: Optimale Spiele: Minimax und alpha-beta-Pruning (4P)





## Games.03: Minimax vereinfachen (1P)

``` python
def Minimax(state):
    if Terminal-Test(state):
        return Utility(state)
    v = -INF
    for (a, s) in Successors(state):
        v = max(v, -Minimax(s)) # rekursiver Aufruf der Maximierungsfunktion mit negativer Knotenbewertung
    return v
```
<br>

``` python
Minimax()
```

## Games.04: Suchtiefe begrenzen (1P)

Die Spielzustände spiegeln direkt wieder, welcher Spieler im Vorteil ist. Das kommt (1) durch die höhere Gewichtung der Zustände zustande, bei denen mit 2 X oder O belegte Zeilen/Spalten/Diagonalen und (2) durch die Berechnung der Eval-Funktion als Nullsummenspiel.

So kann auch mit begrenzter Baumhöhe/Suchtiefe der nächste beste Zug ermittelt werden.

## Games.05: Minimax generalisiert (1P)

