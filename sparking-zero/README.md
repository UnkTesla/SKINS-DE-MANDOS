# Skin: Dragon Ball Sparking Zero (Xbox One) para GamePadViewer

Skin personalizado para mostrar tu control en OBS usando GamePadViewer.

## Estructura
```
sparking-zero/
├── sparking-zero.css     <- el CSS principal
├── assets/               <- todas las imagenes PNG
│   ├── base.png
│   ├── button-a.png / button-a-pressed.png ... (ABXY)
│   ├── stick-left.png / stick-right.png (+ pressed)
│   ├── trigger-left/right.png, bumper-left/right.png
│   ├── dpad-up/down/left/right.png
│   ├── guide.png, start-select.png
```

## Como usarlo

1. Sube TODA la carpeta `sparking-zero/` a tu repositorio de GitHub.
2. Activa GitHub Pages (Settings > Pages > Deploy from branch > main > root).
3. Tu CSS quedara en una URL como:
   `https://TUUSUARIO.github.io/REPO/sparking-zero/sparking-zero.css`
4. Arma la URL de GamePadViewer (usa `css=`, NO `editcss=`):
   `https://gamepadviewer.com/?p=1&s=1&css=https://TUUSUARIO.github.io/REPO/sparking-zero/sparking-zero.css`
5. En OBS: pega esa URL en el campo URL de la fuente Navegador.
   Deja "CSS personalizado" VACIO.

## Notas
- El skin base debe ser Xbox One (s=1).
- Las imagenes usan rutas relativas (assets/), por eso deben subirse
  junto al CSS manteniendo la estructura de carpetas.
- Comportamiento: ABXY y sticks siempre visibles; triggers y bumpers
  aparecen solo al presionar (con su aura azul/naranja); D-pad tenue
  que resalta al presionar.
