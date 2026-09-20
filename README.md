# Splendida Nam

Giochi di matematica per la seconda elementare — numeri fino a 20, costruiti attorno agli **amici del 10**.
Maths games for Year 2 — numbers up to 20, built around the **number bonds to 10**.

**Online:** https://splendidanam.vercel.app

La home di `/` chiede al bambino, in italiano e in inglese, di cliccare sulla propria lingua.
The page at `/` asks the child, in Italian and in English, to click on their own language.

## I giochi / The games

| # | Italiano — `/it/` | English — `/en/` | Cosa allena / What it trains |
|---|-------------------|------------------|------------------------------|
| 01 | [La casa del 10](it/casa-del-10.html) | [The house of 10](en/house-of-10.html) | Le coppie che fanno 10 / Pairs that make 10 |
| 02 | [Il ponte del 10](it/ponte-del-10.html) | [The bridge to 10](en/bridge-to-10.html) | Scomporre per passare dal 10 / Splitting to bridge through 10 |
| 03 | [Colpo d'occhio](it/colpo-docchio.html) | [Quick look](en/quick-look.html) | Riconoscere quantità senza contare / Subitising |
| 04 | [Parte, parte, tutto](it/parte-parte-tutto.html) | [Part, part, whole](en/part-part-whole.html) | La relazione parte-parte-tutto / Part-part-whole |
| 05 | [Quanto manca?](it/quanto-manca-salita.html) | [How many more?](en/how-many-more.html) | La sottrazione come salita / Subtraction as counting up |
| 06 | [Lo specchio dei doppi](it/specchio-dei-doppi.html) | [The doubles mirror](en/doubles-mirror.html) | Doppi, quasi-doppi e metà / Doubles, near doubles, halves |
| 07 | [Catene e Vero / Falso](it/catene-vero-falso.html) | [Chains and True / False](en/chains-true-false.html) | Calcoli in sequenza e il senso dell'uguale / Chains and the meaning of `=` |

## Come funziona

Pagine HTML statiche, una per gioco, senza dipendenze e senza build: si aprono anche facendo doppio clic sul file.

```
index.html      pagina di scelta della lingua / language picker
it/index.html   home italiana + 7 giochi
en/index.html   English home + 7 games
vercel.json     redirect dai vecchi URL alla cartella /it/
```

Le due versioni sono costruite allo stesso modo: stessa grafica, stessa logica di gioco,
stessi punteggi. Cambia solo la lingua dei testi (e il formato della data).
The two versions are built the same way — same look, same game logic, same scoring;
only the wording and the date format change.

I vecchi indirizzi (`/casa-del-10.html` e simili) rimandano automaticamente alla versione italiana.

Ogni push su `main` viene pubblicato automaticamente su Vercel.
