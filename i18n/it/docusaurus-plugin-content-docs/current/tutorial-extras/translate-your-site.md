---
sidebar_position: 2
---

# Traduci il tuo sito

Traduciamo `docs/intro.md` in francese.

## Configura i18n

Modifica `docusaurus.config.js` per aggiungere il supporto per la locale `fr`:

```js title="docusaurus.config.js"
modulo.export = {
  i18n: {
    defaultLocale: 'en',
    locales: ['en', 'fr'],
  },
};
```

## Traduci un documento

Copia il file `docs/intro.md` nella cartella `i18n/fr`:

```bash
mkdir -p i18n/fr/docusaurus-plugin-content-docs/current/

cp docs/intro.md i18n/fr/docusaurus-plugin-content-docs/current/intro.md
```

Traduci `i18n/fr/docusaurus-plugin-content-docs/current/intro.md` in francese.

## Avvia il tuo sito localizzato

Avvia il tuo sito nella lingua francese:

```bash
npm run start -- --locale fr
```

Il tuo sito localizzato è accessibile da `http://localhost:3000/fr/` e la pagina `Getting Started` è tradotta.

:::attenzione

In fase di sviluppo, puoi utilizzare solo un'impostazione internazionale alla volta.

:::

## Aggiungi un menu a discesa delle impostazioni internazionali

Per navigare senza problemi tra le lingue, aggiungi un menu a discesa delle impostazioni internazionali.

Modifica il file `docusaurus.config.js`:

```js title="docusaurus.config.js"
modulo.export = {
  temaConfig: {
    barra di navigazione: {
      Oggetti: [
        // inizio evidenziazione
        {
          digita: 'localeDropdown',
        },
        // evidenzia-fine
      ],
    },
  },
};
```

Il menu a discesa delle impostazioni locali ora appare nella barra di navigazione:

![Dropdown delle impostazioni locali](/img/tutorial/localeDropdown.png)

## Crea il tuo sito localizzato

Crea il tuo sito per una lingua specifica:

```bash
npm run build -- --locale fr
```

Oppure crea il tuo sito per includere tutte le impostazioni locali contemporaneamente:

```bash
npm esegui build
```