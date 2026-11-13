---
version: alpha
name: Aldo Iván — Sistema de Diseño Editorial
description: Portafolio editorial de base clara con firma de peso progresivo, tipografía de carácter y acentos de azul y rosa.
colors:
  primary: "#0C0C0C"
  on-primary: "#F4F4F4"
  secondary: "#4F4F4F"
  tertiary: "#105EF9"
  on-tertiary: "#F4F4F4"
  surface: "#F4F4F4"
  on-surface: "#0C0C0C"
  surface-dark: "#222222"
  on-surface-dark: "#F4F4F4"
  surface-raised: "#393939"
  surface-muted: "#DADADA"
  on-surface-muted: "#222222"
  text-muted-dark: "#BFBFBF"
  accent-graphic: "#0000F4"
  accent-detail: "#EF1889"
typography:
  display-xl:
    fontFamily: DM Sans
    fontSize: 80px
    fontWeight: 700
    lineHeight: 80px
    letterSpacing: -2px # ajustado para DM Sans (antes -4 px con BC Novatica CYR)
  display-xl-mobile:
    fontFamily: DM Sans
    fontSize: 44px
    fontWeight: 700
    lineHeight: 46px
    letterSpacing: -1px
  hero-statement:
    fontFamily: DM Sans
    fontSize: 82px
    fontWeight: 300
    lineHeight: 87px
    letterSpacing: -4px
  hero-statement-mobile:
    fontFamily: DM Sans
    fontSize: 36px
    fontWeight: 300
    lineHeight: 38px
    letterSpacing: -2px
  section:
    fontFamily: DM Sans
    fontSize: 48px
    fontWeight: 700
    lineHeight: 52px
    letterSpacing: -1px # calibrado para DM Sans; el documento original no definía espaciado a 48 px
  section-mobile:
    fontFamily: DM Sans
    fontSize: 32px
    fontWeight: 700
    lineHeight: 36px
    letterSpacing: -1px # calibrado para DM Sans; el documento original no definía espaciado a 32 px
  project:
    fontFamily: DM Sans
    fontSize: 28px
    fontWeight: 700
    lineHeight: 32px
    letterSpacing: 0px
  project-mobile:
    fontFamily: DM Sans
    fontSize: 24px
    fontWeight: 700
    lineHeight: 28px
    letterSpacing: 0px
  subtitle:
    fontFamily: DM Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 26px
    letterSpacing: -1px
  body:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: 400
    lineHeight: 28px
    letterSpacing: 0px
  body-mobile:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: 400
    lineHeight: 25px
    letterSpacing: 0px
  nav:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 20px
    letterSpacing: 0px
  meta:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
    letterSpacing: 0px
  label:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: 500
    lineHeight: 20px
    letterSpacing: 0px
  note:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: 400
    lineHeight: 16px
    letterSpacing: 0px
spacing:
  base: 4px
  xxs: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  xxl: 48px
  xxxl: 64px
  section: 96px
  pause: 128px
  section-tablet: 72px
  section-mobile: 56px
  gutter: 24px
  gutter-tablet: 20px
  margin: 48px
  margin-tablet: 32px
  margin-mobile: 20px
rounded:
  none: 0px
  sm: 4px
  md: 12px
  lg: 16px
  xl: 20px
  full: 9999px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.nav}"
    rounded: "{rounded.md}"
    padding: 16px
    height: 48px
  button-primary-hover:
    backgroundColor: "{colors.surface-raised}"
  button-primary-active:
    backgroundColor: "{colors.surface-dark}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.nav}"
    rounded: "{rounded.md}"
    padding: 16px
    height: 48px
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  button-secondary-active:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-primary}"
  button-accent:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    typography: "{typography.nav}"
    rounded: "{rounded.md}"
    padding: 16px
    height: 48px
  button-accent-hover:
    backgroundColor: "{colors.accent-graphic}"
  button-accent-active:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  dark-secondary-text:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.text-muted-dark}"
    typography: "{typography.meta}"
  hero-portrait:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.note}"
    rounded: "{rounded.none}"
  error-marker:
    backgroundColor: "{colors.accent-detail}"
    rounded: "{rounded.full}"
    size: 8px
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    size: 44px
  tag:
    backgroundColor: "{colors.surface-muted}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.meta}"
    rounded: "{rounded.full}"
    padding: 12px
  tag-selected:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body-mobile}"
    rounded: "{rounded.md}"
    padding: 12px
    height: 48px
  nav-floating:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.nav}"
    rounded: "{rounded.lg}"
  overlay-actions:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-surface-dark}"
    typography: "{typography.nav}"
    rounded: "{rounded.lg}"
  project-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.project}"
    rounded: "{rounded.sm}"
  link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.tertiary}"
    typography: "{typography.body}"
  modal:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.xl}"
---

## Overview

Este sistema describe un portafolio editorial abierto: una composición con tensión, tipografía de carácter, una base neutra y pequeños acentos de cristal. La personalidad es sobria y deja que los proyectos tengan el protagonismo; el recorrido debe ser claro para quien entra a entender qué hago y a encontrar mi trabajo.

El portafolio usa una sola base clara: {colors.surface} para el fondo y {colors.on-surface} para la lectura. Los tonos oscuros permanecen en la paleta solo para bloques puntuales, no como un segundo modo de página.

La firma no está en aplicar un efecto a todo, sino en cómo selecciono, ordeno y relaciono las piezas: el contraste entre un encabezado compacto y una zona amplia de descanso, o entre una imagen dominante y una descripción breve. Letras gruesas y cercanas entre sí, imágenes con protagonismo y pocos recursos bien elegidos.

Cada zona mantiene un solo acento dominante y cada bloque, una sola acción principal. La densidad y los tamaños se resuelven para una pantalla real: los menús se leen y los controles se pueden tocar sin precisión excesiva. Los efectos deben tener una función visible dentro del recorrido; si solo añaden ruido, se eliminan.

Este archivo es la fuente de verdad de la apariencia: los valores de color, tipografía, espaciado, formas y componentes viven aquí. El contenido, el orden de lectura y los enlaces se definen en el documento de arquitectura del portafolio, y cada cambio en ambos se anota en `docs/REGISTRO-CAMBIOS.md`.

## Colors

El fondo principal es {colors.surface} y el texto es {colors.primary}. Esa relación deja que la fotografía y los proyectos aporten variedad. En bloques oscuros se usa {colors.surface-dark} como superficie y {colors.on-surface-dark} para la lectura. {colors.surface-raised} y {colors.secondary} distinguen niveles; {colors.surface-muted} y {colors.text-muted-dark} separan o acompañan contenido sobre fondos claros.

- **Primary (#0C0C0C):** tinta profunda para titulares y texto principal sobre fondos claros.
- **On-primary (#F4F4F4):** lectura sobre tinta profunda y sobre el botón principal.
- **Secondary (#4F4F4F):** texto secundario oscuro y bordes de 1 px en controles.
- **Tertiary (#105EF9):** azul de enlaces y de algunas acciones. Es el único acento de navegación.
- **On-tertiary (#F4F4F4):** texto sobre el azul de acción.
- **Surface (#F4F4F4):** base de la página y de las superficies claras; la base neutra del sistema.
- **Surface-dark (#222222):** superficie de bloques oscuros.
- **Surface-raised (#393939):** nivel intermedio y estado presionado.
- **Surface-muted (#DADADA):** etiquetas y separadores sobre claro.
- **Text-muted-dark (#BFBFBF):** texto secundario sobre superficies oscuras.
- **Accent-graphic (#0000F4):** azul con papel gráfico sobre fondos claros; no se usa en texto pequeño.
- **Accent-detail (#EF1889):** rosa de detalle ocasional, asociado a una pieza o sección. Nunca es un segundo color de navegación.

Contraste: sobre {colors.surface}, {colors.tertiary} alcanza aproximadamente 4.78:1, y la misma relación se mantiene al colocar {colors.on-tertiary} sobre un botón azul. Sobre {colors.primary}, el contraste de {colors.tertiary} baja a 3.72:1 y el de {colors.accent-graphic} a 2.15:1; por eso los enlaces pequeños sobre oscuro se mantienen claros y subrayados. El rosa {colors.accent-detail} queda fuera del texto pequeño sobre fondo claro.

La página usa fondo {colors.surface}, lectura {colors.on-surface} y texto secundario {colors.secondary}. {colors.surface-dark} queda disponible para componentes oscuros puntuales, con {colors.on-surface-dark} como lectura y enlaces claros subrayados. No hay selector de tema.

Un estado activo, un error o un enlace se reconoce también por su forma, su mensaje o un subrayado, no solo por el color. Cada zona mantiene un solo acento dominante.

Los 15 roles cromáticos se construyen con 10 valores únicos. En la guía visual cada valor se muestra una vez con todos sus roles: la repetición de un hexadecimal no crea un color nuevo. Esta distinción evita inflar artificialmente la paleta.

## Typography

**DM Sans** es la voz más visible: Bold concentra la fuerza del nombre y los titulares, y Medium acompaña los subtítulos, la navegación y los botones. **Manrope** Regular se usa en las descripciones y los textos de lectura; su Medium queda disponible para etiquetas que necesitan un poco más de presencia.

Ambas son familias variables y se sirven desde `assets/fonts/` en formato WOFF2: DM Sans cubre pesos de 100 a 1000 y ajusta su tamaño óptico entre 9 y 40 según el tamaño de letra; Manrope cubre pesos de 200 a 800. Con una sola descarga por familia se obtienen todos los pesos del sistema.

| Nivel | Escritorio (tamaño / interlineado) | Móvil (tamaño / interlineado) |
|:--|:--|:--|
| Apertura | 80 / 80 px | 44 / 46 px |
| Sección | 48 / 52 px | 32 / 36 px |
| Proyecto | 28 / 32 px | 24 / 28 px |
| Subtítulo | 20 / 26 px | 20 / 26 px |
| Texto de lectura | 18 / 28 px | 16 / 25 px |
| Menús y botones | 16 / 20 px | 16 / 20 px |
| Metadatos | 14 / 20 px | 14 / 20 px |
| Notas auxiliares | 12 / 16 px | 12 / 16 px |

El primer valor indica el tamaño y el segundo, el interlineado. Las notas auxiliares pueden usar 12 / 16 px siempre que no contengan información esencial.

En titulares de 80 px se reduce el espacio entre letras 2 px ({typography.display-xl.letterSpacing}); en el nombre o en una palabra corta se puede llegar a 3 px después de revisar la unión visual entre caracteres. En titulares de 44 px y en los subtítulos se parte de una reducción de 1 px ({typography.display-xl-mobile.letterSpacing} y {typography.subtitle.letterSpacing}). Los botones y los párrafos conservan el espaciado original.

El ajuste está calibrado para DM Sans: si una letra toca a la siguiente, se abre el espaciado antes que reducir el tamaño del titular. Cada caso se revisa para que las letras no choquen y la lectura siga siendo clara.

Las mayúsculas se concentran en el nombre y en mensajes breves. Los títulos largos pueden ocupar varias líneas y conservan altura suficiente. La jerarquía depende del tamaño, el peso y la posición, con espacio alrededor de cada nivel. Nunca se fuerza una familia sustituta: si DM Sans no está disponible, se conserva la escala y el peso antes que cambiar el carácter tipográfico.

La comparación entre escritorio y móvil muestra los tamaños reales de cada token. El selector y las muestras cambian con una transición de 220 ms; la preferencia por movimiento reducido elimina esa animación.

## Layout

En escritorio se trabaja con 12 columnas, calles de {spacing.gutter} y un ancho de contenido máximo de 1200 px, con márgenes mínimos de {spacing.margin}. Una imagen especial puede extenderse hasta 1440 px, mientras sus textos conservan la alineación principal. Se alternan proyectos de mayor tamaño con otros más contenidos para evitar una sucesión de bloques idénticos.

La retícula parte de una base de 4 px y de la escala {spacing.xxs}, {spacing.xs}, {spacing.sm}, {spacing.md}, {spacing.lg}, {spacing.xl}, {spacing.xxl}, {spacing.xxxl}, {spacing.section} y {spacing.pause}. Dentro de un componente se dejan entre 12 y 24 px; entre bloques relacionados, de 24 a 32 px. Las secciones principales se separan {spacing.section} en escritorio y {spacing.section-mobile} en móvil. {spacing.pause} se reserva para una pausa importante entre temas. Los párrafos mantienen entre 55 y 70 caracteres por línea.

Puntos de quiebre:

- **Menos de 600 px:** una columna con márgenes de {spacing.margin-mobile}; bloques relacionados separados 16 px y secciones a {spacing.section-mobile}.
- **De 600 a 1023 px:** 8 columnas, márgenes de {spacing.margin-tablet}, calles de {spacing.gutter-tablet} y separaciones principales de {spacing.section-tablet}.
- **Desde 1024 px:** retícula de 12 columnas y secciones separadas {spacing.section}.
- **Desde 1440 px:** el contenido se mantiene centrado dentro del ancho definido.

En móvil se reordenan las composiciones asimétricas según su importancia. La navegación puede condensarse en un menú rotulado; las barras flotantes respetan las zonas seguras y dejan espacio para no tapar el final de la página. Los elementos esenciales funcionan con toque y teclado, además del cursor.

Las portadas provisionales de los proyectos usan marcos rectangulares con radio {rounded.xl}. El módulo presenta una vista principal grande y cuatro miniaturas superpuestas en la base: portada, sistema, detalle y aplicación. Cada miniatura cambia la vista principal y tiene un área de control amplia. El azul {colors.tertiary} marca una vista de acento y el rosa {colors.accent-detail} solo un indicador pequeño; las imágenes reales conservarán su color. El cristal se reserva para la navegación y una etiqueta flotante de estado sobre el módulo, nunca para cubrir texto de lectura.

## Elevation & Depth

La profundidad se concentra en la navegación flotante y, cuando se necesita, en una barra de acciones superpuesta a una imagen. En la página clara se usa {colors.surface} al 88 %, desenfoque de fondo de 16 px y borde de 1 px en {colors.primary} al 12 %. El texto y los íconos permanecen completamente opacos.

Las fotografías, los proyectos y los formularios conservan superficies sólidas. No se acumulan capas transparentes en una misma zona. Si el fondo dificulta la lectura o se desactiva la transparencia, la navegación usa {colors.surface} sólido.

Sombras permitidas:

- Navegación flotante: desplazamiento horizontal 0 px, vertical 4 px, desenfoque 16 px, {colors.primary} al 8 %.
- Menú: 0 px, 8 px y 24 px, al 12 %.
- Modales: opacos, con un velo negro al 40 % detrás.
- Tarjetas de proyecto: sin sombra permanente; se integran al fondo.

Las transiciones duran entre 160 y 220 ms y se concentran en color, borde y pequeños cambios de escala o posición. Al solicitar movimiento reducido se eliminan los desplazamientos y los aumentos de imagen. La portada admite un ciclo breve del personaje, sin sonido y sin controles, porque presenta la faceta de movimiento del autor. No se repiten animaciones decorativas en los proyectos.

## Shapes

Los redondeos se concentran en los controles y las capas flotantes. Botones y campos usan {rounded.md} (12 px); la navegación y los contenedores destacados, {rounded.lg} (16 px); los modales, {rounded.xl} (20 px). Las portadas conservan bordes rectos ({rounded.none}) o un radio de {rounded.sm} (4 px).

La forma de píldora ({rounded.full}) queda para filtros y etiquetas; los círculos, para avatares y controles de ícono. Las imágenes mantienen una geometría más contenida para conservar el carácter editorial.

El nombre funciona como firma tipográfica; no se incorporan símbolos decorativos ajenos a la identidad.

## Components

**Navegación.** Flota sobre el contenido con el tratamiento de cristal descrito en Elevation & Depth y usa nombres directos: Proyectos, Sobre mí y Contacto. Los enlaces se leen a {typography.nav}; el destino activo se distingue por peso, posición o subrayado, no solo por color.

**Presentación y proyectos.** La entrada combina el logotipo vectorial del nombre con un juego progresivo de pesos, del trazo ligero de la «a» al negro de la «n», y sitúa el personaje a su lado. La frase «me gusta entender una idea antes de darle forma» lleva el peso de la presentación; «idea» y «forma» parten en DM Sans Light; al pasar el cursor cambian con un fundido breve a DM Sans Medium Italic y toman {colors.tertiary} y {colors.accent-detail}. En dispositivos táctiles los acentos permanecen visibles sin depender del cursor. Debajo, un texto breve nombra la condición de estudiante y el proceso de observación y prueba. Dos acciones conducen a Sobre mí y Proyectos. Sobre mí precede a los proyectos; después, los proyectos ocupan la mayor parte del recorrido y el contacto lo cierra. El personaje aparece solo en la entrada para que no compita con las imágenes de los trabajos. Cada proyecto abre con su nombre, categoría y año. La explicación conecta el problema con la idea y las decisiones visuales antes de mostrar las aplicaciones. Se incluye la participación y los créditos cuando el trabajo es compartido.

**Tarjetas de proyecto.** Cada entrada reúne una imagen, el nombre, la categoría y el año, separados entre 12 y 16 px. La imagen y el título abren el mismo destino. Al pasar el cursor se subraya el nombre y la imagen puede crecer hasta un 2 % dentro de su marco. La fotografía personal puede ser monocromática; las piezas del portafolio conservan los colores que necesitan para entenderse. Sin sombra permanente.

**Botones.** El botón principal usa {components.button-primary.backgroundColor} con texto {components.button-primary.textColor}, altura mínima de {components.button-primary.height}, espacio horizontal de {components.button-primary.padding} y radio de {rounded.md}. Al pasar el cursor sube a {components.button-primary-hover.backgroundColor} y al presionarlo baja a {components.button-primary-active.backgroundColor}; el cambio de luminosidad es visible para que el reposo y el hover no se confundan. Sobre oscuro se usa la versión clara. El botón azul {components.button-accent.backgroundColor} se reserva para una acción que requiera énfasis, mantiene texto {components.button-accent.textColor} y al pasar el cursor cambia a {components.button-accent-hover.backgroundColor}; al presionarlo pasa a {components.button-accent-active.backgroundColor} con texto {components.button-accent-active.textColor}.

**Botones secundarios y controles de ícono.** Los secundarios tienen fondo claro, texto oscuro y borde de 1 px en {colors.secondary}; al pasar el cursor invierten a {components.button-secondary-hover.backgroundColor} con texto {components.button-secondary-hover.textColor}, y al presionarlos usan {components.button-secondary-active.backgroundColor}. Los controles de ícono disponen de un área mínima de 44 × 44 px y un nombre accesible.

**Retrato del personaje.** La portada usa una animación transparente de cinco segundos derivada del video original. Se reproduce en bucle, sin sonido ni controles; al preferir menos movimiento se muestra una imagen fija. La transparencia permite que {colors.surface} sea el único fondo y evita un recuadro alrededor del dibujo. El personaje aparece junto a la firma, una sola vez y sin marco. Es una pieza personal, no un trabajo de cliente.

**Mensajes de error.** El texto explica el problema junto al campo y se acompaña de un punto de {components.error-marker.size} en {components.error-marker.backgroundColor}; el color no es la única señal. El texto secundario sobre oscuro usa {components.dark-secondary-text.textColor}.

**Etiquetas y filtros.** Las etiquetas usan {components.tag.backgroundColor} con texto {components.tag.textColor} a {typography.meta.fontSize} / {typography.meta.lineHeight} y forma de píldora. Los filtros seleccionados invierten a fondo oscuro y texto claro ({components.tag-selected.backgroundColor} y {components.tag-selected.textColor}).

**Enlaces.** En fondo claro, los enlaces usan {components.link.textColor} y se reconocen por el subrayado. Sobre fondos oscuros se mantienen claros y subrayados; el azul no se usa en texto pequeño sobre oscuro.

**Contacto y formularios.** El contacto ofrece una acción directa y reconocible. Si se incluye un formulario, los campos miden al menos 48 px de alto y usan fondo {components.input.backgroundColor}, texto {components.input.textColor} y borde de 1 px en {colors.secondary}. Las etiquetas visibles van a 14 / 20 px; el texto de ejemplo nunca las sustituye. El foco incorpora un contorno azul sobre claro y uno claro sobre oscuro. Los errores aparecen explicados junto al campo.

**Modales.** Son opacos, con radio {rounded.xl}, texto {components.modal.textColor} sobre {components.modal.backgroundColor}, y un velo negro al 40 % detrás.

Los encabezados, muestras y componentes se animan individualmente cada vez que entran en el área visible y se restablecen al salir, con desplazamiento vertical máximo de 36 px y fundido de 620 ms. El contenido permanece disponible sin JavaScript y se muestra de inmediato cuando se solicita movimiento reducido. La página abre desde la portada, salvo que se siga un enlace directo a una sección. Esta entrada acompaña el recorrido; no altera el orden de lectura.

## Do's and Don'ts

- **Sí:** mantener una acción principal por bloque y un solo acento dominante por sección.
- **No:** convertir el rosa {colors.accent-detail} en un segundo color de navegación ni usarlo en texto pequeño sobre fondo claro.
- **Sí:** conservar el color de las imágenes de los proyectos cuando forma parte del trabajo.
- **No:** aplicar el efecto de cristal a párrafos, formularios o a todas las tarjetas; se reserva para la navegación y las acciones flotantes.
- **Sí:** mantener los títulos compactos con fuerza, sin perder legibilidad ni desbordar la pantalla.
- **No:** usar el azul en texto pequeño sobre fondos oscuros; los enlaces mantienen subrayado y los estados incluyen señales adicionales al color.
- **Sí:** sostener el contraste WCAG AA (4.5:1) en texto normal y ofrecer una superficie sólida cuando no haya transparencia.
- **No:** acumular capas transparentes en una misma zona ni añadir sombra permanente a las tarjetas de proyecto.
- **Sí:** respetar la preferencia de movimiento reducido, eliminando desplazamientos y aumentos de imagen.
- **No:** incorporar animaciones continuas en los proyectos; el ciclo breve del personaje queda reservado a la portada y se detiene con la preferencia de movimiento reducido.
- **Sí:** revisar qué aporta cada recurso, qué hace más fácil y si conserva la claridad en móvil.
- **Sí:** mantener una única base clara y reservar {colors.surface-dark} para bloques puntuales.
- **No:** introducir un selector de tema ni colores ajenos a la paleta.
- **No:** añadir símbolos decorativos ajenos a la identidad tipográfica del nombre.
