---
sidebar_position: 1
---

# Italian Manage Docs Versions

Docusaurus può gestire più versioni dei tuoi documenti.

## Crea una versione di documenti

Rilascia una versione 1.0 del tuo progetto:

```bash
npm esegui docusaurus docs: versione 1.0
```

La cartella "docs" viene copiata in "versioned_docs/version-1.0" e viene creato "versions.json".

I tuoi documenti ora hanno 2 versioni:

- `1.0` in `http://localhost:3000/docs/` per i documenti della versione 1.0
- `current` su `http://localhost:3000/docs/next/` per i **documenti non rilasciati in arrivo**

## Aggiungi una versione a discesa

Per navigare senza problemi tra le versioni, aggiungi un menu a discesa delle versioni.

Modifica il file `docusaurus.config.js`:

```js title="docusaurus.config.js"
modulo.export = {
  temaConfig: {
    barra di navigazione: {
      Oggetti: [
        // inizio evidenziazione
        {
          digita: 'docsVersionDropdown',
        },
        // evidenzia-fine
      ],
    },
  },
};
```

Il menu a discesa della versione dei documenti viene visualizzato nella barra di navigazione:

![Dropdown versione documenti](/img/tutorial/docsVersionDropdown.png)

## Aggiorna una versione esistente

È possibile modificare i documenti con versione nella rispettiva cartella:

- `versioned_docs/version-1.0/hello.md` aggiorna `http://localhost:3000/docs/hello`
- `docs/hello.md` aggiorna `http://localhost:3000/docs/next/hello`