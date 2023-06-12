# Bootstrap Italia Playground

Questo progetto è il modo più semplice per iniziare ad usare [Bootstrap Italia](https://italia.github.io/bootstrap-italia/).

Il playground per la vecchia versione di Bootstrap Italia è disponibile sul [branch 1.x](https://github.com/italia/bootstrap-italia-playground/tree/1.x).

<img src="https://github.com/italia/bootstrap-italia-playground/blob/1.x/bootstrap-italia-playground.png?raw=true" width="800"> 

## Cos'è incluso

Troverai una semplice pagina HTML con i riferimenti ai file di Bootstrap Italia e con file CSS e JS vuoti per iniziare.

```
bootstrap-italia-playground/
│   index.html          # main html file
├── css/
│   ├── main.css        # working CSS file
└── js/
    └── main.js         # working JS file
```

## Come lanciare l'ambiente in locale

* Installa le dipendenze: `npm install`
* Compila l'applicazione: `npm run build`
* Lancia un server locale: `npm run serve`
* Vai all'indirizzo: `http://127.0.0.1:8080/` e continua a leggere.

## Personalizzare i colori di Bootstrap Italia

Per personalizzare i colori di Bootstrap Italia, fai riferimento al file `scss/bootstrap-italia-custom.scss`, dove il colore `$primary` è sovrascritto nelle sue componenti.
Per ottenere una versione personalizzata della libreria:

* Compila la libreria Bootstrap Italia personalizzata con: `npm run build`
* La compilazione crea dei file nella cartella `css/compiled` che vanno referenziati nell file `index.html`
* Nel file `index.html` commenta il file CSS della libreria Bootstrap Italia originale `<link href="/node_modules/bootstrap-italia/dist/css/bootstrap-italia.min.css" rel="stylesheet">`
* Nel file `index.html` decommenta il file CSS delle libreria Bootstrap Italia personalizzata `<link href="/css/bootstrap-italia-custom.min.css" rel="stylesheet">`

Lanciando di nuovo il sito con `npm run serve`, il sito dovrebbe diventare rosso! 😉

## Cambiamenti dalla versione Bootstrap Italia 2.3.0

Da [Bootstrap Italia v2.3.0](https://github.com/italia/bootstrap-italia/releases/tag/v2.3.0) abbiamo introdotto nuove variabili semantiche (collegate alla prossima integrazione dei token di progettazione).

Queste variabili sono:

```sss
$color-background-primary-lighter
$color-text-primary-active
$color-text-primary-hover
```

Sono dichiarate in `_colors_vars.scss` ([dalla riga 392](https://github.com/italia/bootstrap-italia/blob/main/src/scss/utilities/colors_vars.scss)) e sovrascritte ad esempio in `bootstrap-italia-comuni.scss` [(linee 26-28)](https://github.com/italia/bootstrap-italia/blob/main/src/scss/bootstrap-italia-comuni.scss)

Alcuni componenti adesso usano queste variabili invece di quelle vecchie (come `$neutral-` o `complementary-`).

Per impostare correttamente il tema dell'installazione BI, è necessario assegnare un valore al tema. È possibile utilizzare i valori HEX, HSL o HSB.

## Riferimento

La documentazione di Bootstrap Italia è presente su GitHub pages all'indirizzo https://italia.github.io/bootstrap-italia/docs/come-iniziare/personalizzazione-della-libreria/.

