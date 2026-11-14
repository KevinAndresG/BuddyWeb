# Buddy – sitio web

Página promocional y guía de uso de [Buddy](https://github.com/KevinAndresG/PersonalAssistant). Un solo `index.html` estático, sin build.

## Ver en local

```bash
python -m http.server 5181
```

Abrir http://localhost:5181

## Publicar (GitHub Pages)

1. Crear el repo en GitHub y subir: `git remote add origin https://github.com/KevinAndresG/BuddyWeb.git && git push -u origin main`
2. En el repo: *Settings → Pages → Source: Deploy from a branch → main / (root)*.
3. Queda en `https://kevinandresg.github.io/BuddyWeb/`.

También sirve tal cual en Netlify, Vercel o Cloudflare Pages (arrastrar la carpeta).

## Botón de descarga

Apunta a `https://github.com/KevinAndresG/PersonalAssistant/releases/latest`. Para que funcione, el repo de la app debe ser público y tener un *Release* con `Buddy Setup x.y.z.exe` adjunto (`npm run dist` en el proyecto de la app).
