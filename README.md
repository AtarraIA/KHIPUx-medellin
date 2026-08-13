# KHIPUx Medellín

Sitio web estático de **KHIPUx Medellín — Bienestar, Educación e IA**, publicado con GitHub Pages.

**Sitio:** https://atarraia.github.io/KHIPUx-medellin/

Página única con portada y las secciones *Acerca de*, *Programación* e *Inscripción*,
siguiendo la guía visual del evento: paleta navy + coral, acuarela azul–roja, motivos
circulares y arte botánico de fondo.

## Estructura

- `index.html` — página única con la portada y las tres secciones.
- `style.css` — estilos responsivos, sin paso de compilación.
- `assets/` — imágenes, logos y fuentes (ver abajo).
- `.nojekyll` — desactiva el procesamiento de Jekyll; los archivos se sirven tal cual.
- `.gitignore` — ignora la configuración local de edición (`.claude/`) y archivos del sistema.

### `assets/`

| Archivo | Uso |
| --- | --- |
| `LogoKHIPUMedellin.svg` | Logo circular del encabezado. |
| `BotanicalKHIPUmedellin.svg` | Arte botánico de fondo (portada y panel de *Programación*). |
| `DetallesCircularesKHIPU.svg` | Fila de 5 motivos circulares (acuarela enmascarada por sus formas). |
| `watercolor.jpg` | Banda acuarela del pie de página. |
| `LogoKHIPU.svg`, `LogoAtarraia.svg`, `LogoUniversidadNacional.svg` | Logos del pie de página (versión blanca). |
| `Coloreado.pdf` | Acuarela original (fuente del diseño; el sitio no la carga directamente). |
| `fonts/HeadingNow-74*.woff2` | Fuente *Heading Now 74* auto-alojada. |

## Tipografía

- **Open Sans** (título de portada y contenido) se carga desde Google Fonts.
- **Heading Now 74** (títulos de sección y subtítulo) va **auto-alojada** en `assets/fonts/`.

> ⚠️ **Heading Now es una fuente comercial.** Los `.woff2` incluidos son *subconjuntos*
> que solo contienen los glifos del texto actual; existe *fallback* a Open Sans para
> cualquier carácter nuevo. Si se cambia un título a una palabra con letras que no estén
> en el subconjunto, esas letras no se verán en Heading Now. Para textos nuevos, reemplazar
> por el archivo completo de la fuente (conservando el nombre en la regla `@font-face`) y
> verificar la licencia de uso web.

## Editar el contenido

Los textos provisionales están marcados con `[Texto pendiente]` o `[Por definir]` dentro de
`index.html`. Basta con reemplazarlos y hacer commit: GitHub Pages vuelve a publicar
automáticamente en un par de minutos.

Para la inscripción, reemplazar el enlace `mailto:` del botón *Inscribirme* por la URL del
formulario cuando esté disponible.

## Vista previa local

```sh
python -m http.server 8000
# abrir http://localhost:8000
```

## Contacto

atarraiaredesneuronales@gmail.com
