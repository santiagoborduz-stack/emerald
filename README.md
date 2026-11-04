# Guerras Esmeralderas · Archivo vivo

Sitio de investigación sobre el conflicto esmeraldero colombiano. Reúne dos piezas:

| Archivo | Qué es |
| --- | --- |
| `index.html` | Sitio editorial: territorio, cuatro claves del conflicto, autor, cronología, clanes, esmeralderos y narcos. |
| `mapeo.html` | Aplicación interactiva de mapeo: fichas de actores, red de conexiones, importación de Excel y edición. |
| `data.js` | Datos iniciales de `mapeo.html`. Por ahora es una base vacía. |
| `README.md` | Esta guía. |

## Ver el sitio

Abre `index.html` con doble clic. No necesita servidor.

- La página principal es el archivo editorial.
- El botón o enlace a `mapeo.html` abre la aplicación de mapeo.
- La aplicación también funciona abriendo `mapeo.html` directamente.

Requiere conexión a internet para las librerías y tipografías externas (Tailwind, Lucide, Google Fonts, SheetJS y vis-network).

## La aplicación de mapeo

En `mapeo.html`:

- **Mapeo**: haz clic en un personaje y luego en cada conexión para seguir el hilo.
- **Actores**: búsqueda, filtros, tarjetas o tabla, ficha completa.
- **Hechos**: cronología filtrable.
- **Datos**: importar Excel/CSV/JSON, exportar, descargar plantilla y descargar `data.js`.
- Todo se guarda en el navegador (`localStorage`, clave `guerras-esmeralderas-mapeo-v2`).

La base está vacía a propósito para que cargues tu propia estructura de actores, vínculos, hechos y categorías.

## Publicar en GitHub Pages

1. Crea un repositorio público, por ejemplo `guerras-esmeralderas`.
2. Sube `index.html`, `mapeo.html` y `data.js`.
3. Entra a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
5. Guarda. GitHub publica el sitio en `https://TU-USUARIO.github.io/guerras-esmeralderas/`.

El mapeo interactivo queda en `https://TU-USUARIO.github.io/guerras-esmeralderas/mapeo.html`.

## Actualizar los datos del mapeo

1. Abre `mapeo.html` e importa el Excel.
2. Corrige fichas, vínculos y hechos.
3. En **Datos**, pulsa **Descargar data.js**.
4. Reemplaza `data.js` en el repositorio.
5. Haz commit. GitHub Pages actualiza el sitio.

## Respaldo local

`data-respaldo.js` conserva la importación anterior del archivo de investigación (37 actores, 63 vínculos y 116 hechos). No forma parte del sitio público; sirve como copia de seguridad local. Si necesitas recuperarla, renómbrala a `data.js` o pídeme que la reconecte.

## Notas

- El sitio editorial tiene sus datos y textos integrados en `index.html`.
- La aplicación de mapeo no envía archivos a ningún servidor: el Excel se procesa en el navegador.
- Los tipos de actor y las categorías se pueden ajustar cuando definas la taxonomía definitiva.
