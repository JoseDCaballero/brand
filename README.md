# Parbok · Logo en partículas

Escena interactiva con [three.js](https://threejs.org): el logo de Parbok formado por miles de partículas brillantes, con sus propios colores.

- **Mueve el cursor o el dedo** sobre el logo: las partículas se apartan con un remolino y luego regresan a su lugar.
- **Haz clic o toca** para dispersar todo el logo; se vuelve a armar solo.
- Las partículas se ensamblan al cargar la página, el logo se inclina siguiendo el puntero y hay polvo de fondo con bloom.

## Cambiar el logo

- Reemplaza `logo.jpg` (o cambia `LOGO` en la configuración de `index.html`). Funciona mejor con fondo liso o transparente: el color de las esquinas se toma como fondo y se descarta.
- `MIN_LIGHTNESS` aclara los tonos oscuros para que brillen sobre el fondo oscuro.
- Modo texto: `index.html?text=TU%20MARCA` (usa `PALETTE` como gradiente).

## Ejecutar en local

three.js se carga desde un CDN, así que no hace falta instalar nada. Ábrelo con un servidor local (abrir el archivo directo no deja leer los píxeles del logo):

```bash
npx serve .
# o
python3 -m http.server
```

Luego abre `http://localhost:3000` (o `:8000`).

## Publicar

Funciona directo en GitHub Pages: Settings → Pages → Deploy from branch → `main` / root.
