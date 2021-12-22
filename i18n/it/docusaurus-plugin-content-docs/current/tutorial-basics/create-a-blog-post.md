---
sidebar_position: 3
---

# Italian Create a Blog Post

Docusaurus crea una **pagina per ogni post**, ma anche una **pagina indice del blog**, un **sistema di tag**, un **feed RSS**...

## Crea il tuo primo post

Crea un file su `blog/2021-02-28-greetings.md`:

```md title="blog/2021-02-28-greetings.md"
---
lumaca: saluti
titolo: Saluti!
autori:
   - nome: Joel Marcey
     titolo: Co-creatore di Docusaurus 1
     URL: https://github.com/JoelMarcey
     image_url: https://github.com/JoelMarcey.png
   - nome: Sébastien Lorber
     titolo: manutentore di Docusaurus
     URL: https://sebastienlorber.com
     image_url: https://github.com/slorber.png
tag: [saluti]
---

Congratulazioni, hai scritto il tuo primo post!

Sentiti libero di giocare e modificare questo post quanto vuoi.
```

Un nuovo post sul blog è ora disponibile su `http://localhost:3000/blog/greetings`.