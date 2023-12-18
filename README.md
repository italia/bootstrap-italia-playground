# Bootstrap Italia Playground

Questo progetto è il modo più semplice per iniziare ad usare [Bootstrap Italia](https://italia.github.io/bootstrap-italia/).

Il playground per la vecchia versione di Bootstrap Italia è disponibile sul [branch 1.x](https://github.com/italia/bootstrap-italia-playground/tree/1.x).

<img src="https://github.com/italia/bootstrap-italia-playground/blob/main/.github/bootstrap-italia-playground.png?raw=true" width="800"> 

## Cos'è incluso

Troverai una semplice pagina HTML con i riferimenti ai file di Bootstrap Italia e con file CSS e JS vuoti per iniziare.

```
bootstrap-italia-playground/
│   index.html          # main html file
├── scss/
│   ├── _custom_.scss   # working SCSS file
└── js/
    └── main.js         # working JS file
```

## Come lanciare l'ambiente in locale

* Installa le dipendenze: `npm install`
* Lancia un server locale: `npm run serve` (auto refresh ad ogni cambiamento)
* Vai all'indirizzo: `http://127.0.0.1:3000/`.

## Personalizzare i colori di Bootstrap Italia

Per personalizzare i colori di Bootstrap Italia, fai riferimento al file `scss/_custom.scss`, dove il colore `$primary` è sovrascritto nelle sue componenti.
Lanciando di nuovo il sito con `npm run serve`, il sito dovrebbe diventare rosso! 😉

## Cambiamenti dalla versione Bootstrap Italia 2.3.0

Da [Bootstrap Italia v2.3.0](https://github.com/italia/bootstrap-italia/releases/tag/v2.3.0) abbiamo introdotto nuove variabili semantiche (collegate alla prossima integrazione dei token di progettazione).

Queste variabili sono:

```scss
$color-background-primary-lighter
$color-text-primary-active
$color-text-primary-hover
```

Sono dichiarate in `_colors_vars.scss` ([dalla riga 392](https://github.com/italia/bootstrap-italia/blob/main/src/scss/utilities/colors_vars.scss)).
Alcuni componenti adesso usano queste variabili invece di quelle vecchie (come `$neutral-` o `complementary-`).

Per impostare correttamente il tema dell'installazione BI, è necessario assegnare un valore al tema. È possibile utilizzare i valori HEX, HSL o HSB.

## Riferimento

La documentazione di Bootstrap Italia è presente su GitHub pages all'indirizzo https://italia.github.io/bootstrap-italia/docs/come-iniziare/personalizzazione-della-libreria/.

