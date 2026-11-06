# Fase 1: Análisis

## 1. Perfiles de referencia

- [thmsgbrt](https://github.com/thmsgbrt/thmsgbrt)
- [jvillegasd](https://github.com/jvillegasd/Jvillegasd)
- [CyrisXD](https://github.com/CyrisXD/CyrisXD)

## 2. Comparación de perfiles

| Criterio | thmsgbrt | jvillegasd | CyrisXD |
|----------|----------|------------|---------|
| **Presentación (primeros 10 s)** | Saludo breve; se presenta como desarrollador fullstack, con su origen y dónde vive ahora. | Título "Hi, I'm Johnny" y subtítulo "software engineer from Colombia". Claro y directo. | Cabecera animada con nombre y rol (desarrollador, maker, infosec) y un párrafo con intereses y ubicación. |
| **Estructura y jerarquía** | Saludo, tecnologías, proyectos open source, últimas publicaciones, sección de ciudad (clima y fotos), contacto. Algunas secciones no aportan al perfil profesional. | Tech stack agrupado por categoría, hobbies, proyectos actuales, estado de Spotify. Orden lógico y fácil de escanear. | Cabecera, redes, presentación, proyecto actual, blog, herramientas, trabajos previos, estadísticas. |
| **Habilidades** | Insignias de tecnologías (shields.io). No son verificables por sí solas. | Íconos agrupados por categoría; el texto alternativo lista los nombres. No son verificables por sí solos. | Íconos de herramientas con texto alternativo. No son verificables por sí solos. |
| **Proyectos fijados y descripción** | Tabla de 3 proyectos open source con estrellas, forks, issues y PRs. | Solo listó "proyectos actuales" en texto, sin enlaces. | Proyecto actual con imagen, 2 repositorios en tarjetas y 4 artículos del blog. |
| **Contacto** | Insignias de GitHub, Twitter, LinkedIn y Medium al final. | No tiene un canal o enlaces de contacto en el README. | Twitter, sitio web, Mastodon y insignias de redes. |
| **Accesibilidad y móvil** | Depende de imágenes y servicios externos; muchas insignias; contenido automático (clima, fotos) que puede quedar desactualizado. | Buen texto alternativo; el widget de Spotify depende de un servicio propio. | El texto de la cabecera está dentro de un GIF; las estadísticas dependen de servicios externos. |

## 3. Revisión de repositorios fijados

Repositorios revisados:

- [react-simple-pull-to-refresh](https://github.com/thmsgbrt/react-simple-pull-to-refresh) (thmsgbrt)
- [nodejs-typescript-express-apollo-graphql-starter](https://github.com/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter) (thmsgbrt)
- [love-lock-card](https://github.com/CyrisXD/love-lock-card) (CyrisXD)

| Característica | react-simple-pull-to-refresh | nodejs-typescript-express-apollo-graphql-starter | love-lock-card |
|----------------|------------------------------|--------------------------------------------------|----------------|
| **Descripción corta, topics y enlace a demo/sitio** | La descripción es solo el comando de instalación; el campo de sitio apunta al paquete en npm y el README enlaza a una demo en GitHub Pages. | La descripción invita a leer el tutorial y el sitio enlaza a ese tutorial en Medium. | Descripción clara de lo que hace (tarjeta de Home Assistant que bloquea tarjetas con contraseña o confirmación). Sin sitio ni topics visibles. |
| **README** | Muy completo: insignias (npm, licencia, tipos), qué es, demo, instalación, uso con código, tabla de props y changelog con créditos a colaboradores. Sin capturas. | Mínimo: título y un enlace al tutorial. Toda la explicación vive fuera del repositorio. | Completo: aviso de mantenimiento, descripción y advertencia de seguridad, GIF de ejemplo, tabla de opciones, instalación, ejemplos de configuración y créditos. |
| **Licencia y `.gitignore`** | Licencia MIT (el archivo se llama `LICENCE`) y `.gitignore`. | `.gitignore`; sin archivo de licencia. | Licencia MIT; sin `.gitignore`. |
| **Historial de commits** | 122 commits. Parte del historial son actualizaciones automáticas de dependencias. | 12 commits.| 21 commits. |
| **Issues, PRs, ramas y Releases** | 9 issues y 18 PRs abiertos, con colaboradores externos acreditados en el changelog. Sin releases publicadas. | 8 PRs abiertos; 47 estrellas y 11 forks. Sin releases. | 19 issues y 1 PR abiertos; 153 estrellas y 15 forks. Sin releases. |
| **Estructura de carpetas** | Organizada: `src`, `docs`, `playground`, `.vscode` y archivos de configuración (`package.json`, `tsconfig.json`, `rollup.config.js`, `.prettierrc.yaml`). | `src`, `.vscode` y configuración (`package.json`, `tsconfig.json`, `.prettierrc`). | Plana y mínima: `love-lock-card.js`, `hacs.json`, `README.md` y `LICENSE`. |

### Lo que me llevo para mis repositorios

- Un README con propósito, instalación, uso y un ejemplo visual (como el de love-lock-card) se entiende sin salir de GitHub; el que depende de un tutorial externo deja al visitante con poca información.
- La licencia y el `.gitignore` son detalles pequeños que dan sensación de proyecto cuidado.
- Una descripción corta que diga qué hace el proyecto (no solo cómo instalarlo) ayuda a que los repos fijados se entiendan a primera vista.
- Un aviso honesto sobre el estado del proyecto (en mantenimiento, sin nuevas funciones) evita expectativas falsas.

## 4. Requisitos de mi perfil

### Requisitos funcionales

- Mostrar en las primeras líneas mi nombre, rol y ubicación.
- Incluir una sección de habilidades agrupada por categorías.
- Destacar de 3 a 4 proyectos, cada uno con su ficha (problema, tecnologías, enlace al repo y a la demo si existe).
- Ofrecer al menos un canal de contacto visible.
- Estar publicado también como sitio en GitHub Pages.

### Requisitos no funcionales

- **Legibilidad:** secciones cortas y con jerarquía clara; que se lea bien en móvil.
- **Accesibilidad:** texto alternativo en las imágenes, nada de texto importante dentro de imágenes, buen contraste.
- **Mantenibilidad:** solo Markdown, sin depender de servicios externos para información esencial, y commits pequeños con mensajes descriptivos.