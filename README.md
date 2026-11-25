# Brand · Partículas

Escena interactiva con [three.js](https://threejs.org): el nombre de la marca formado por miles de partículas brillantes.

- **Mueve el cursor o el dedo** sobre el logo: las partículas se apartan con un remolino y luego regresan a su lugar.
- **Haz clic o toca** para dispersar todo el logo; se vuelve a armar solo.
- Las partículas se ensamblan al cargar la página, el logo se inclina siguiendo el puntero y hay polvo de fondo con bloom.

## Cambiar el texto

- Desde la URL: `index.html?text=TU%20MARCA`
- O en el código, en la sección de configuración de `index.html` (`TEXT` y `PALETTE`).

## Ejecutar en local

Es un solo archivo HTML. three.js se carga desde un CDN, así que no hace falta instalar nada:

```bash
npx serve .
# o
python3 -m http.server
```

Luego abre `http://localhost:3000` (o `:8000`).

## Publicar

Funciona directo en GitHub Pages: Settings → Pages → Deploy from branch → `main` / root.
