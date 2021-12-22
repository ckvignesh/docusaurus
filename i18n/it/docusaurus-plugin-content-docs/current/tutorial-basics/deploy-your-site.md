---
sidebar_position: 5
---

# Italian Deploy your site

Docusaurus è un **generatore di siti statici** (chiamato anche **[Jamstack](https://jamstack.org/)**).

Costruisce il tuo sito come semplici **file HTML, JavaScript e CSS statici**.

## Crea il tuo sito

Costruisci il tuo sito **per la produzione**:

```bash
npm esegui build
```

I file statici vengono generati nella cartella `build`.

## Distribuisci il tuo sito

Testa la tua build di produzione in locale:

```bash
npm esegui servizio
```

La cartella `build` è ora disponibile in `http://localhost:3000/`.

Ora puoi distribuire la cartella `build` **quasi ovunque** facilmente, **gratuitamente** o con un costo molto ridotto (leggi la **[Guida alla distribuzione](https://docusaurus.io/docs/deployment)* *).