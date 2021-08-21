# Electronics shop

*Livello: facile*

Questo esercizio è stato preso a piene mani da [hackerrank](https://www.hackerrank.com/challenges/electronics-shop/problem)

## Problema

Ginetto vuole comprare una tastiera ed una penna USB, e vuole riuscire a spendere il più possibile con il budget che ha a disposizione.

Ad esempio:
- budget (`b`) = 60
- costi\_tastiere = `[40, 50, 60]`
- costi\_penne\_usb = `[5, 8, 12]`

Gino potrà comprare la tastiera da 40 + la usb da 12 (= 52) o la tastiera da 50 e la usb da 8 (= 58).
Opterà per quest'ultima ipotesi in quanto quella più costosa.

L'output desiderato è la cifra che Ginetto spenderà, o -1 nel caso non ci sia niente a disposizione con la limitazione del budget.

Per maggiori informazioni e qualche test già a disposizione, si rimanda [all'esercizio originale](https://www.hackerrank.com/challenges/electronics-shop/problem).

## Opportunità

- Essendo questo un esercizio abbastanza semplice, si raccomanda anche di scrivere l'implementazione per la lettura da `stdin` e la scrittura su `stdout`, così da fare pratica con queste funzionalità.
- Cercate di scrivere codice idiomatico (ad esempio, il fatto che l'output debba essere -1 non vuol dire che la funzione che elabora i soldi spesi debba necessariamente tornare un intero con segno).
- Il codice può andare in `panic`, ma questo dovrebbe poter succedere solo nella main (per questo esercizio, non in generale). Implementate quindi le varie funzionalità in modo tale che non vadano in `panic`. Bonus: integrate una gestione degli errori.
- Utilizzate gli strumenti a disposizione: Rust Analyzer, Clippy e possibilmente Rustfmt
- Bonus 1: integrate degli unit test per constatare l'affidabilità dell'implementazione.
- Bonus 2: integrate dei benchmark per valutare la velocità di esecuzione e permettere miglioramenti evitando regressions.
- Bonus 3 (avanzato): fate fuzzing della vostra implementazione. Potete trovare [qui](https://rust-fuzz.github.io/book/) maggiori informazioni.
