# P*tas Startups

Blog editorial sin filtros sobre el ecosistema startup.

## Setup local

```bash
# Instalar Hugo extended (v0.140+)
brew install hugo

# Clonar y arrancar
git clone <repo> && cd putas-startups
hugo server -D
```

Abre `http://localhost:1313`

## Crear un nuevo post

```bash
hugo new posts/nombre-del-post.md
```

Edita el archivo en `content/posts/` con tu editor favorito. Los posts se escriben en Markdown.

## Deploy en Cloudflare Pages

1. Conecta el repo de GitHub en Cloudflare Pages
2. Build command: `hugo --minify`
3. Build output directory: `public`
4. Environment variable: `HUGO_VERSION` = `0.140.2`

Cada push a `main` despliega automaticamente.

## Estructura

```
content/
  posts/          # Posts del blog
  manifiesto/     # Pagina del manifiesto
  sobre/          # Pagina sobre el blog
themes/
  putas-theme/    # Tema personalizado
```
