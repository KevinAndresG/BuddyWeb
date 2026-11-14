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

Descarga directa: `https://github.com/KevinAndresG/PersonalAssistant/releases/latest/download/Buddy-Setup.exe`. Siempre apunta al último Release, así que la web no cambia al sacar versiones nuevas. El asset debe llamarse exactamente `Buddy-Setup.exe`:

```powershell
npm run dist
Copy-Item "dist\Buddy Setup X.Y.Z.exe" dist\Buddy-Setup.exe
gh release create vX.Y.Z dist\Buddy-Setup.exe --title "Buddy X.Y.Z" --notes "..."
```
