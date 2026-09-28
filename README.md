# Portafolio | Heimy Romero

One page en HTML5 y CSS3: semántica, responsive, con modo claro/oscuro e imágenes en WebP.

## Estructura

```text
index.html
css/styles.css
img/heimy-400.webp
img/heimy-800.webp
```

Agrega tus archivos `heimy-400.webp` y `heimy-800.webp` dentro de `img/` antes de publicar.

## Git Flow + Conventional Commits

Ejecuta estos comandos desde la carpeta `portafolio/`:

```bash
git init
git add .
git commit -m "chore: 🎉 commit inicial"
git branch -M main
git remote add origin https://github.com/rheimydaniela-wq/portafolio.git
git push -u origin main

git switch -c develop
git push -u origin develop

git switch -c feature/estructura-html
git add index.html
git commit -m "feat: ✨ agrega estructura semántica"
git switch develop
git merge --no-ff feature/estructura-html

git switch -c feature/estilos
git add css/styles.css
git commit -m "style: 💄 agrega estilos responsive"
git switch develop
git merge --no-ff feature/estilos

git switch main
git merge --no-ff develop
git push origin main develop
```

Otros ejemplos: `docs: 📝 agrega README`, `perf: ⚡ optimiza imágenes a webp`, `fix: 🐛 corrige menú en móvil`.

## Despliegue en GitHub Pages

En el repositorio: **Settings → Pages → Deploy from a branch → `main` / `(root)` → Save**.
El sitio queda en `https://rheimydaniela-wq.github.io/portafolio/`.