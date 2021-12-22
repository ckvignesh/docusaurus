---
sidebar_position: 2
---

# Italian Create a Document

I documenti sono **gruppi di pagine** collegati tramite:

- una **barra laterale**
- **navigazione precedente/successiva**
- **versione**

## Crea il tuo primo documento

Crea un file markdown su `docs/hello.md`:

```md title="docs/hello.md"
# Ciao

Questo è il mio **primo documento Docusaurus**!
```

Un nuovo documento è ora disponibile su `http://localhost:3000/docs/hello`.

## Configura la barra laterale

Docusaurus **crea automaticamente una barra laterale** dalla cartella `docs`.

Aggiungi metadati per personalizzare l'etichetta e la posizione della barra laterale:

```md title="docs/hello.md" {1-4}
---
sidebar_label: 'Ciao!'
sidebar_position: 3
---

# Ciao

Questo è il mio **primo documento Docusaurus**!
```

È anche possibile creare esplicitamente la barra laterale in `sidebars.js`:

```diff title="sidebars.js"
modulo.export = {
   tutorialSidebar: [
     {
       tipo: 'categoria',
       etichetta: 'Tutorial',
-     Oggetti: [...],
+ elementi: ['ciao'],
     },
   ],
};
```