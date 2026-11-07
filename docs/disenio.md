# Fase 2: Planificación y diseño

## 1. Estructura del perfil

Orden de las secciones del `README.md`, de arriba hacia abajo:

1. **Presentación:** nombre, rol y una frase que diga qué hago.
2. **Sobre mí:** 2 o 3 líneas sobre mi formación y lo que estoy aprendiendo.
3. **Habilidades y tecnologías:** agrupadas por categoría.
4. **Proyectos destacados:** de 3 a 4 fichas.
5. **Contacto:** correo, LinkedIn y otros canales.

Secciones del plan que **no** voy a usar y por qué:

- *Áreas de interés:* Se integrará en "Sobre mí"
- *Actividad o experiencia:*  la incluiré dentro de proyectos

Esquema del archivo:

```markdown
# [Nombre] 👋
[Rol] | [Una frase sobre lo que hago]

## Sobre mí
[2 o 3 líneas]

## Habilidades y tecnologías
| Categoría | Tecnologías |
|-----------|-------------|
| Lenguajes | |
| Frontend | |
| Herramientas | |

## Proyectos destacados
### MIJO
### Festival Perla del Pacífico
### ResQ-Mesh

## Contacto
- Correo:
- LinkedIn:
```

## 2. Diseño del contenido

| Sección | Qué incluiré | Qué evitaré | Formato | Enlaces necesarios | Lectura rápida |
|---------|--------------|-------------|---------|--------------------|----------------|
| Presentación | Nombre, rol, frase corta | Texto largo o datos personales sensibles | Título y una línea | Ninguno | Lo esencial en las primeras 2 líneas |
| Sobre mí | Estudiante de Ing. en Computación en Ecuador, aprendiendo sobre desarrollo web | Párrafos largos, frases genéricas | Texto corto | Ninguno | Máximo 3 líneas |
| Habilidades | Solo tecnologías que he usado en proyectos | Listas enormes de insignias (solo esenciales), tecnologías que apenas conozco | Tabla por categoría con nombres en texto | Ninguno | Categorías claras y nombres escritos |
| Proyectos destacados | Ficha de cada proyecto (ver sección 4) | Proyectos sin README o sin terminar | Subtítulo y lista por proyecto | Repositorio y demo | 4 o 5 líneas por proyecto |
| Contacto | Correo electrónico, LinkedIn | Canales que no reviso | Lista | Correo, LinkedIn, etc. | Visible al final, con íconos |

Decisiones generales de diseño:

- Todo en Markdown; sin HTML ni CSS.
- Las imágenes llevarán texto alternativo, y nada importante irá escrito *dentro* de una imagen.
- Evitaré depender de servicios externos para información esencial (estadísticas, widgets).
- El orden de la página sigue lo que más interesa a quien me visita: quién soy, qué sé hacer, qué he construido, cómo contactarme.

## 3. Estrategia de commits

Usaré [Commits Convencionales](https://www.conventionalcommits.org/es/v1.0.0-beta.2/): `tipo: descripción corta en minúsculas`.

| Tipo | Cuándo lo uso |
|------|---------------|
| `docs:` | Cambios de contenido en documentos y README |
| `feat:` | Agregar una sección o un proyecto nuevo |
| `fix:` | Corregir errores (ortografía, enlaces rotos) |
| `chore:` | Estructura inicial u organización del repositorio |

Reglas:

- Un commit por cambio importante; nunca todo el trabajo en uno solo.
- Reviso el resultado en GitHub antes de pasar al siguiente cambio.
- Mensajes en español, descriptivos y en tiempo presente.

## 4. Fichas de proyectos destacados

### Proyecto 1: MIJO, asistente de voz para verificar noticias

- **Problema o necesidad que resuelve:** ayuda a verificar información y noticias hablando con un asistente, sin tener que escribir. Diseñado para adultos mayores.
- **Tecnologías utilizadas:** React, Vite, Node.js y Express, Web Speech API (reconocimiento y síntesis de voz) y la API de Anthropic para generar las respuestas.
- **Funcionalidades principales:** reconocimiento de voz real, respuestas habladas, respuestas generadas por IA, chat con historial, adjuntar imagen o enlace y minijuegos educativos.
- **Mi aporte:** La etapa de ideación de la aplicación fue junto a mis compañeros, y luego me encargué de desarrollar el diseño del prototipo y la app funcional.
- **Repositorio:** https://github.com/Vale-gc/mijo-app
- **Demostración:** Puedes probar la app web en el enlace: [MIJO](https://mijo-frontend.onrender.com)

### Proyecto 2: Landing page del Festival Perla del Pacífico

- **Problema o necesidad que resuelve:** difunde un festival cultural de música clásica realizado en el Centro Cívico de Guayaquil y acerca el evento a la comunidad.
- **Tecnologías utilizadas:** HTML, CSS y JavaScript sobre la plantilla Story de HTML5 UP, con Git y GitHub (ramas y pull requests) para el control de versiones.
- **Funcionalidades principales:** sitio de una sola página adaptable a móvil, con secciones del festival, artistas, director, programa, lugar, galería y contacto.
- **Mi aporte:** Realicé principalmente los cambios en el HTML, escogiendo entre los estilos que ofrecía la plantilla y editando el contenido.
- **Repositorio:** https://github.com/Vale-gc/perla-pacifico-web
- **Demostración:** https://vale-gc.github.io/perla-pacifico-web/

### Proyecto 3: ResQ-Mesh, red de rescate sin conexión

- **Problema o necesidad que resuelve:** después de un terremoto, sin torres celulares ni internet, permite que una persona atrapada pida ayuda golpeando tres veces y que el centro de mando reciba la alerta.
- **Tecnologías utilizadas:** JavaScript (módulos ES, sin frameworks), Web Audio API, BroadcastChannel API (red mesh simulada), HTML5 y CSS.
- **Funcionalidades principales:** detección de tres golpes por el micrófono, botón de SOS manual, envío de alertas como paquetes por la red, lista de triaje ordenada por urgencia, sirena de respuesta y marcado de sectores atendidos.
- **Mi aporte:** realicé el código del estado global del sistema y la conexión entre todas las partes (audio, canales, paquetes, interfaz) a través de store.js y app.js.
- **Repositorio:** https://github.com/Geannesan/CS_Hackathon
- **Demostración:** funciona en local con un servidor simple.

## Referencias

- Commits Convencionales. (n.d.). *Commits Convencionales*. https://www.conventionalcommits.org/es/v1.0.0-beta.2/
