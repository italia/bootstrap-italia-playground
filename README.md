# Bootstrap Italia Playground

Questo progetto è il modo più semplice per iniziare ad usare [Bootstrap Italia](https://italia.github.io/bootstrap-italia/).

<img src="https://github.com/italia/bootstrap-italia-playground/blob/master/bootstrap-italia-playground.png" width="800"> 

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

* Clona o scarica il repository: `git clone https://github.com/italia/bootstrap-italia-playground.git`
* Installa le dipendenze: `yarn install`
* Lancia un server locale: `yarn start`
* Vai all'indirizzo: `http://127.0.0.1:8080/` e continua a leggere.

## Personalizzare i colori di Bootstrap Italia

Per personalizzare i colori di Bootstrap Italia, fai riferimento al file `scss/bootstrap-italia-custom.scss`, dove il colore `$primary` è sovrascritto nelle sue componenti.
Per ottenere una versione personalizzata della libreria:

* Compila la libreria Bootstrap Italia personalizzata con: `yarn buildCSS`
* La compilazione crea dei file nella cartella `css/compiled` che vanno referenziati nell file `index.html`
* Nel file `index.html` commenta il file CSS della libreria Bootstrap Italia originale `<link href="/node_modules/bootstrap-italia/dist/css/bootstrap-italia.min.css" rel="stylesheet">`
* Nel file `index.html` decommenta il file CSS delle libreria Bootstrap Italia personalizzata `<link href="/css/bootstrap-italia-custom.min.css" rel="stylesheet">`

Lanciando di nuovo il sito con `yarn start`, il sito dovrebbe diventare rosso! 😉

## Riferimento

La documentazione di Bootstrap Italia è presente su GitHub pages all'indirizzo https://italia.github.io/bootstrap-italia/docs/come-iniziare/personalizzazione-della-libreria/.

