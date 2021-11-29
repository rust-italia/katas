# Alfametica 

Per chi volesse approfondire l'alfametica può farlo [qui](https://en.wikipedia.org/wiki/Verbal_arithmetic) (in inglese).

## Problema

I problemi di alfametica si basano sulla sostituzione di parole con numeri.

Per esempio `SEND + MORE = MONEY`:
```
  S E N D
  M O R E +
-----------
M O N E Y
```

Sostituendo queste lettere con dei numeri validi si ottiene:
```
  9 5 6 7
  1 0 8 5 +
-----------
1 0 6 5 2
```

I numeri scelti sono validi poiché ogni lettera è sostituita da un numero diverso e la somma delle parole, trasformate in numeri, da il risultato corretto.

Ogni lettera deve rappresentare un numero diverso e, qualora la parola fosse composta da più di una lettera, la prima non può diventare uno zero.

## Richieste

Scrivere una funzione che:

1. Data una stringa della forma `A + B = C`, dove `A`, `B` e `C` sono parole, trovi una soluzione valida per `C` secondo le regole precedentemente descritte e restituisca la somma risultante;

2. Data una stringa della forma `A0 + A1 + ... + An = B`, dove `A0`, `A1`, ..., `An` e `B` sono parole, trovi una soluzione valida per `B` secondo le regole precedentemente descritte e restituisca la somma risultante.

### Nota

Con "parole" si intende sequenze di caratteri ASCII composte solo da lettere maiuscole. Volendo si può pensare di gestire nella propria soluzione ulteriori casistiche.

Non ci sono vincoli sulla rappresentazione del risultato.

## Obiettivi secondari

Risolvere l'esercizio usando la *forza bruta* è sicuramente fattibile ma porterebbe degli svantaggi a livello di efficienza. Prova a trovare una soluzione più complessa.

Evita di riscrivere quanto più possibile funzioni già presenti nella std (in particolare quelle per la manipolazione delle stringhe).

Non limitarti al channel stable di Rust, potresti trovare utile e/o stimolante l'uso di [GAT]s nella tua soluzione.

[GAT]: https://github.com/rust-lang/rfcs/blob/master/text/1598-generic_associated_types.md

---

Link all'[originale](https://exercism.org/tracks/haskell/exercises/alphametics).