# DAM1M04-Exercici004 — Reproducción de Strata

> **Aviso académico:** Este proyecto es una reproducción académica realizada con fines exclusivamente educativos para el módulo M04 (Lenguajes de Marcas).

## Estructura del proyecto

```
DAM1M04-Exercici004/
├── index.html
├── formulario.html
├── estils.css
├── assets/
│   ├── img/
│   │   ├── nexus-screenshot.png
│   │   ├── nexus-screenshot.webp
│   │   ├── search.svg
│   │   ├── strata-icon.png
│   │   ├── strata-icon.svg
│   │   └── strata-logo.svg
│   └── js/
│       ├── hero-graph.js
│       └── vendor/
│           ├── 3d-force-graph.min.js
│           ├── 3d-force-graph-LICENSE.txt
│           ├── three.min.js
│           └── three-LICENSE.txt
└── README.md
```

## Cómo abrir y visualizar la página

1. Clona o descarga este repositorio manteniendo intacta la estructura de carpetas (en especial la carpeta `assets/` con sus subdirectorios).
2. Abre el archivo `index.html` directamente en cualquier navegador web moderno (Chrome, Firefox, Edge, Safari) o ejecútalo mediante un servidor local (como *Live Server* en VS Code o desde el servidor Proxmox del instituto).
3. No se requiere conexión a internet para visualizar la web, ya que todos los recursos gráficos y librerías JavaScript se cargan de forma local desde el propio proyecto.

## Decisiones de adaptación responsive (móvil y tableta)

Se ha verificado y adaptado el diseño para las resoluciones de **1440 px**, **768 px**, **390 px**, aplicando las siguientes decisiones:

* **Reorganización del layout:** Uso de CSS Grid y Flexbox en `estils.css` para adaptar las cuadrículas y bloques de contenido de múltiples columnas a una sola columna en pantallas pequeñas.
* **Sección Hero y gráfico 3D:** En escritorio se ejecuta la animación interactiva controlada por `assets/js/hero-graph.js` asegurando que no interfiera ni tape los enlaces. En versión móvil se oculta el gráfico 3D para optimizar el rendimiento y la lectura, conservando únicamente el fondo degradado.
* **Tipografía y espaciados:** Ajuste proporcional de tamaños de texto, márgenes y rellenos para evitar desbordamientos horizontales, solapamientos o cortes de contenido en dispositivos estrechos.
* **Navegación y accesibilidad:** Revisión de los enlaces internos (incluyendo el acceso a `formulario.html`) y mantenimiento de los estilos de foco para garantizar una navegación fluida mediante teclado.

## Procedencia de los recursos

* **Diseño, logotipos, imágenes y textos:** Proceden de la página web oficial de [Strata](https://strata.ai), utilizados únicamente como material de referencia para esta práctica académica.
* **Recursos gráficos locales:** Almacenados en `assets/img/` en formatos optimizados (`.svg`, `.webp`, `.png`) para evitar cualquier dependencia externa de los servidores de Strata.
* **Scripts y librerías de terceros:** La animación 3D de la cabecera se gestiona mediante `assets/js/hero-graph.js` apoyándose en las librerías **Three.js** (`three.min.js`) y **3D Force-Directed Graph** (`3d-force-graph.min.js`), incluidas en local dentro de `assets/js/vendor/` junto con sus respectivas licencias.
