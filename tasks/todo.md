# TODO

- [x] Analizar limitación de Google Sites para incrustación de HTML externo.
- [x] Crear versión alternativa del sitio para embed sin modificar `index.html`.
- [x] Verificar cambios estáticos en el archivo (`min-height` dinámico + ajuste de contenedor).
- [x] Documentar cómo publicarla y usarla en Google Sites.

## Resultado

Se creó `google-sites.html` como versión específica para incrustar en Google Sites sin modificar `index.html`.

Ajustes aplicados en la copia:
- Hero principal con `min-height: calc(var(--vh, 1vh) * 100)` para evitar recortes en iframe.
- Script de corrección de `vh` en `resize` para entornos embebidos.
- Ajustes de padding/ancho para que el contenido aproveche mejor el contenedor de Google Sites.

Uso recomendado:
1. Publicar `google-sites.html` en GitHub Pages (como ruta adicional, por ejemplo `/google-sites.html`).
2. En Google Sites, incrustar esa URL en una sección de ancho completo.
3. Estirar el bloque incrustado al máximo permitido por Sites.
