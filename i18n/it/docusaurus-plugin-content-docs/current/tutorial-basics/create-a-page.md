---
sidebar_position: 1
---

# Italian Create a Page

Aggiungi i file **Markdown o React** a `src/pages` per creare una **pagina autonoma**:

- `src/pages/index.js` -> `localhost:3000/`
- `src/pages/foo.md` -> `localhost:3000/foo`
- `src/pages/foo/bar.js` -> `localhost:3000/foo/bar`

## Crea la tua prima pagina React

Crea un file in `src/pages/my-react-page.js`:

```jsx title="src/pages/my-react-page.js"
import Reagire da 'reagire';
importa layout da '@theme/Layout';

esporta la funzione predefinita MyReactPage() {
   Restituzione (
     <Layout>
       <h1>La mia pagina React</h1>
       <p>Questa è una pagina React</p>
     </Layout>
   );
}
```

Una nuova pagina è ora disponibile su `http://localhost:3000/my-react-page`.

## Crea la tua prima pagina Markdown

Crea un file in `src/pages/my-markdown-page.md`:

```mdx title="src/pages/my-markdown-page.md"
# La mia pagina Markdown

Questa è una pagina Markdown
```

Una nuova pagina è ora disponibile su `http://localhost:3000/my-markdown-page`.