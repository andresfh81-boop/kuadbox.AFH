# Configurador KÜADBOX-400 (PWA offline)

App instalable en el móvil (PWA) para configurar placas y generar el plano técnico de toldos KÜADBOX-400. Funciona sin conexión una vez instalada.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser público o privado).
2. Sube este contenido:
```
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git branch -M main
git push -u origin main
```
3. En GitHub: **Settings → Pages → Source → Deploy from a branch → main / (root)**.
4. Espera 1-2 minutos. La URL será `https://TU_USUARIO.github.io/TU_REPO/`.

## Instalar en el móvil

1. Abre esa URL con el navegador del móvil (Chrome en Android, Safari en iPhone).
2. Android/Chrome: aparece un aviso "Instalar" en la propia app, o menú ⋮ → "Instalar aplicación" / "Añadir a pantalla de inicio".
3. iPhone/Safari: botón compartir → "Añadir a pantalla de inicio".
4. A partir de ahí funciona sin conexión, con icono propio.

## Actualizar la app

Cada vez que cambies `index.html`, sube los cambios (`git add -A && git commit -m "..." && git push`) y sube en 1 el número de `CACHE_NAME` en `sw.js` (p. ej. `kuadbox-v2`) para que los móviles descarguen la versión nueva.
