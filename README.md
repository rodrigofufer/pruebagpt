# Sitio estático — Reparaciones PC a Domicilio (Boca del Río, Veracruz)

Este repositorio contiene un sitio web estático simple para un negocio de reparación de computadoras a domicilio que cubre Boca del Río, todo Veracruz y la Riviera Veracruzana.

Archivos principales:

- `index.html` — página principal con lista de precios y contacto.
- `styles.css` — estilos básicos y responsive.

Instrucciones rápidas para probar localmente:

1. Abrir una terminal en la carpeta del proyecto.
2. Ejecutar un servidor HTTP local (ejemplo con Python 3):

```bash
python3 -m http.server 8000
```

3. Abrir `http://localhost:8000` en el navegador.

Notas y pasos siguientes recomendados:
- Reemplazar el número de teléfono y email en `index.html` por los reales.
- Añadir un logo y fotos propias en vez de imágenes remotas.
- Para desplegar en producción, usar Netlify, Vercel o GitHub Pages.

Despliegue automático con GitHub Pages

- He incluido un workflow de GitHub Actions en `.github/workflows/deploy.yml` que publica automáticamente el contenido del repositorio en GitHub Pages cuando se hace push a la rama `main`.
- Requisitos mínimos: el repositorio debe estar en GitHub y la acción tendrá permiso para crear la publicación de Pages.
- URL esperada: si tu repositorio es público y el owner es `rodrigofufer`, la página suele estar disponible en `https://rodrigofufer.github.io/pruebagpt` una vez que la acción termine la primera publicación. También puedes ver la URL en Settings → Pages del repositorio.

Cómo controlar el despliegue

- Revisar ejecuciones: pestaña "Actions" → seleccionar "Deploy to GitHub Pages" para ver logs.
- Si quieres usar un dominio personalizado, añade un archivo `CNAME` con tu dominio o configura el dominio en Settings → Pages.

Si prefieres desplegar en Netlify o Vercel en lugar de GitHub Pages, dímelo y preparo la configuración (req. token/permiso para conexión automática).