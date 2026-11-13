# Registro de cambios del portafolio

Este archivo existe para que el diseño del sitio, `DESIGN.md` y el documento de arquitectura no se contradigan cuando cambies de opinión. Cada decisión se anota aquí con su fecha, el motivo y los archivos que hay que tocar.

## Quién manda en qué

| Tema | Documento dueño | Qué contiene |
|:--|:--|:--|
| Apariencia | `DESIGN.md` | Colores, tipografías, espaciado, radios, sombras, componentes y reglas visuales. |
| Contenido y estructura | `Arquitectura_portafolio_Aldo_Iván.docx` | Objetivo, recorrido, navegación, secciones, proyectos, textos y criterios de publicación. |
| Implementación | `styles/fonts.css`, `assets/` | Archivos reales y variables que el navegador usa. |

`design.html` es una vista derivada de `DESIGN.md`: muestra los tokens y componentes, pero no inventa valores propios. Si algo difiere, manda `DESIGN.md`.

**Regla de conflicto:** si un valor visual y una decisión de contenido se contradicen, la apariencia la decide `DESIGN.md` y el contenido lo decide el documento de arquitectura. Se corrige el documento que no manda y se anota el cambio aquí. Nunca se dejan dos versiones distintas del mismo dato.

## Versión actual

| Elemento | Estado | Fecha |
|:--|:--|:--|
| Sistema de diseño | v1.2 | 9 de noviembre de 2026 |
| Arquitectura | v1.0 (sin cambios de contenido) | — |
| Tipografías | DM Sans y Manrope, variables, WOFF2 | 9 de noviembre de 2026 |
| Validación oficial | 0 errores, 0 advertencias; 23 componentes | 9 de noviembre de 2026 |

## Historial

### 9 de noviembre de 2026 — Tema claro y oscuro (v1.2)

**Antes:** una sola apariencia clara. Los bloques oscuros eran piezas aisladas, no un tema.

**Ahora:** un interruptor en la cabecera alterna entre tema claro y oscuro. No se añadieron colores: el tema oscuro reasigna los tokens existentes (`surface-dark` como fondo, `on-surface-dark` para lectura, `text-muted-dark` para secundario). Los enlaces sobre oscuro se mantienen claros y subrayados.

**Motivo:** dar una lectura cómoda en entornos oscuros sin duplicar el sistema ni romper el contraste.

**Detalles:**
- Transición de 320 ms sobre color, borde, sombra y filtro; se desactiva con movimiento reducido.
- La preferencia se guarda en `localStorage` (`aldo-theme`) y se aplica antes del primer pintado.
- El botón usa `aria-pressed`, nombres “Activar modo oscuro” y “Activar modo claro”, y actualiza `theme-color`.
- Las ilustraciones del personaje invierten su tinta en oscuro para integrarse al fondo.

**Archivos afectados:**
- `DESIGN.md`: párrafos de Overview, Colors, Elevation y Components; componentes `theme-toggle`, `theme-toggle-dark` y `dark-secondary-text`.
- `design.html`: capa semántica de tokens, botón de tema, bloque de documentación de temas y lógica de persistencia.
- `assets/darkmode.svg` y `assets/lightmode.svg`: íconos del interruptor, embebidos en el HTML.

### 9 de noviembre de 2026 — Retrato animado del personaje (v1.2)

**Antes:** la portada no tenía retrato; la pieza del personaje solo aparecía como tarjeta de proyecto.

**Ahora:** la portada incluye `assets/video/yo-saludo.mp4`, una animación de 5 segundos del personaje saludando, con póster `assets/yo_personaje.png` y controles propios de reproducir, pausar y repetir. La reproducción la inicia la persona; nunca es automática.

**Motivo:** dar presencia personal al sistema sin presentar al personaje como una marca de cliente.

**Detalles:** el video se exportó de `yo.mov` (ProRes 4444, 17 MB) a H.264 sobre `#DADADA`, 700 × 1080, unos 325 KB. El fondo claro se conserva en ambos temas y en oscuro se invierte con CSS.

**Archivos afectados:**
- `assets/video/yo-saludo.mp4`: versión web del video.
- `design.html`: retrato, póster, controles y estilos.
- `DESIGN.md`: componente `hero-portrait` y párrafo “Retrato del personaje”.

### 9 de noviembre de 2026 — Estados de botón más evidentes (v1.2)

**Antes:** el hover del botón principal era casi idéntico al reposo y el botón de acento no tenía estado propio.

**Ahora:**
- Principal: reposo `primary`, hover `surface-raised` (`#393939`), presionado `surface-dark`.
- Secundario: reposo claro con borde, hover invierte a `primary` con texto `on-primary`, presionado `surface-dark`.
- Acento: reposo `tertiary`, hover `accent-graphic` (`#0000F4`), presionado `primary`.

**Motivo:** que el cambio de estado se perciba a simple vista y funcione igual en ambos temas.

**Archivos afectados:**
- `DESIGN.md`: componentes `button-primary-hover`, `button-primary-active`, `button-secondary-hover`, `button-secondary-active`, `button-accent-hover`, `button-accent-active` y párrafos de Components.
- `design.html`: tokens `--btn-*` para ambos temas y estilos de hover, activo y foco.

### 9 de noviembre de 2026 — Tarjeta personal, no de marca (v1.2)

**Antes:** la tarjeta de ejemplo usaba la ilustración del personaje con la categoría “Branding” y el nombre “TipoFilicko”.

**Ahora:** la tarjeta se rotula “Sobre mí / Aldo Iván” y explica que el personaje representa al autor.

**Motivo:** evitar que una pieza personal se confunda con un trabajo de marca para un cliente.

**Archivos afectados:**
- `design.html`: tarjeta y texto de apoyo de la sección Componentes.

### 9 de noviembre de 2026 — Sustitución de tipografías (v1.1)

**Antes:** BC Novatica CYR (titulares) y Neue Haas Grotesk (texto). Ambas comerciales, disponibles solo mediante Adobe Fonts o licencia de autoalojamiento.

**Ahora:** DM Sans (titulares) y Manrope (texto). Licencia SIL Open Font License, archivos propios en `assets/fonts/`.

**Motivo:** eliminar la dependencia de una suscripción y de una licencia web de pago, sin cambiar la intención editorial del sistema.

**Archivos afectados:**
- `DESIGN.md`: `fontFamily` de los 13 niveles tipográficos y párrafos de Typography y Overview.
- `styles/fonts.css`: reglas `@font-face` y variables de familia.
- `assets/fonts/`: `dm-sans-variable.woff2` (87 KB) y `manrope-variable.woff2` (53 KB), más sus licencias.

**Qué se conserva:** la escala de tamaños, los pesos (500 para acompañar, 700 para titular), la jerarquía y el resto del sistema visual.

### 9 de noviembre de 2026 — Ajuste de interletrado (v1.1)

**Antes:** −4 px a 80 px y −2 px a 44 px, valores calibrados para BC Novatica CYR.

**Ahora:** −2 px a 80 px y −1 px a 44 px. Sin cambios en sección (48 px), sección móvil (32 px) y subtítulo (20 px), que ya estaban en −1 px.

**Motivo:** DM Sans es más ancha; con −4 px las letras de "ALDO IVÁN" se tocaban. El ajuste mantiene el gesto compacto sin perder legibilidad.

**Archivos afectados:**
- `DESIGN.md`: tokens `display-xl` y `display-xl-mobile`, y el párrafo de interletrado.
- `styles/fonts.css`: variables `--tracking-display` y `--tracking-display-mobile`.

### 9 de noviembre de 2026 — Página de referencia del sistema (`design.html`)

**Qué es:** una sola página HTML, CSS y JS vanilla que muestra la paleta con el rol de cada color, la escala tipográfica con sus fuentes, el espaciado, la retícula, la elevación, los radios y muestras de componentes. Está construida solo con los tokens de `DESIGN.md` y enlaza `styles/fonts.css` para no duplicar los `@font-face`.

**Decisiones de fidelidad:**
- El botón de acento usa únicamente `tertiary`; no se añadió un color de hover derivado que no exista en `DESIGN.md`.
- Los contrastes de la tabla se calculan en vivo con la fórmula WCAG a partir de los pares de tokens, incluidos los que no cumplen AA.
- La página respeta movimiento reducido, ofrece enlace para saltar al contenido, navegación por teclado, foco visible y regiones con etiqueta.

**Verificación:** 0 errores de consola, fuentes DM Sans y Manrope cargadas, sin desbordamiento horizontal a 320, 390, 888 y 1440 px. Las capturas móviles se hicieron con emulación real de viewport (Chrome headless recorta si se le pide un ancho menor de 500 px, así que no sirve para validar móvil).

**Archivos afectados:**
- `design.html`: página nueva.
- `styles/fonts.css`: se enlaza tal cual, sin cambios.

## Pendientes

| Pendiente | Estado | Nota |
|:--|:--|:--|
| Actualizar el documento de arquitectura | En espera | Está abierto en Word; se actualizará cuando se cierre, para no perder cambios. |
| Revisar el interletrado en el sitio real | Pendiente | La prueba se hizo en una página aislada; falta verlo con los textos y anchos definitivos. |
| Resolver las 3 advertencias de color | Resuelto en v1.2 | `text-muted-dark`, `accent-graphic` y `accent-detail` ya están asociados a componentes; el linter queda en 0 advertencias. |

## Cómo mantener la congruencia

Antes de cambiar algo, revisa esta lista:

1. **Un color** → cámbialo en `colors` de `DESIGN.md`, revisa los componentes que lo usan y su contraste, y anota la fecha aquí.
2. **Una tipografía** → cambia `typography` en `DESIGN.md`, actualiza `@font-face` y las variables de `styles/fonts.css`, y reemplaza los archivos de `assets/fonts/`.
3. **Un tamaño o interletrado** → cambia el token en `DESIGN.md` y su variable `--tracking-*` en el CSS.
4. **Espaciado, radios o sombras** → `spacing`, `rounded` y el bloque de elevación en `DESIGN.md`; luego el CSS.
5. **Estructura, secciones, navegación o textos** → documento de arquitectura; si toca un componente visual, también `DESIGN.md`.
6. **Al terminar** → vuelve a pasar el linter oficial. Debe seguir en 0 errores.

Cada entrada nueva del historial debe responder tres preguntas: **qué cambió**, **por qué** y **qué archivos hay que actualizar**.

## Texto listo para el documento de arquitectura

Cuando cierres Word, este párrafo se añade al final de la introducción del documento de arquitectura:

> Este documento describe el contenido y la estructura del portafolio. Los valores visuales —color, tipografía, espaciado, formas y componentes— se definen en `DESIGN.md`, que es la fuente de verdad de la apariencia; aquí no se repiten para evitar contradicciones. La tipografía se sirve con DM Sans para titulares y Manrope para el texto de lectura, en formato WOFF2 desde `assets/fonts/`. Los cambios de cualquiera de los dos documentos se anotan en `docs/REGISTRO-CAMBIOS.md`.


## 9 de noviembre de 2026 — Congruencia de la guía visual y los documentos

- La guía agrupa 15 roles de color en 10 tonos únicos; el sistema de diseño y el documento de criterios visuales explican la diferencia entre valor y función.
- Las muestras distinguen DM Sans para titulares y controles de Manrope para lectura. La arquitectura mantiene ese reparto y conserva el orden de información en móvil y escritorio.
- El selector de escala usa una transición de 220 ms y respeta movimiento reducido.
- La pieza personal aparece sin marco en su tarjeta; no se presenta como caso de cliente.
- La arquitectura explicita qué datos debe contener cada proyecto y la guía visual mantiene esas reglas visibles.

## 9 de noviembre de 2026 — Ilustración estática y entrada de secciones

- Se retiró el video del retrato y sus controles. La portada y la tarjeta personal usan la ilustración normal en claro y `yo-invertido.svg` en oscuro.
- Cada sección entra una vez con 18 px de desplazamiento y 520 ms de fundido. Sin JavaScript o con movimiento reducido, el contenido se muestra de inmediato.
- `DESIGN.md`, la página visual y ambos documentos de evaluación se actualizaron con la misma decisión. Las entradas anteriores se conservan como historial, no como especificación vigente.

## 9 de noviembre de 2026 — Repetición del movimiento y nueva ilustración

- Se sustituyó la variante blanca por el archivo actualizado del autor.
- La entrada de cada sección se repite al volver a ella: 24 px y 440 ms. Con movimiento reducido no se anima.
- Al abrir la página sin un enlace directo a una sección, el recorrido comienza en la portada.
- Esta decisión sustituye la regla anterior de entrada única y queda reflejada en la página, el sistema y ambos documentos de evaluación.

## 9 de noviembre de 2026 — Movimiento visible por elemento

- La observación de secciones completas se sustituyó por entrada y salida de encabezados, muestras y componentes. La entrada usa 36 px y 620 ms, y se repite en cada recorrido.
- La regla de movimiento reducido permanece: el contenido se muestra sin transición.
- Este ajuste sustituye la duración y distancia de la entrada anterior.

## 9 de noviembre de 2026 — Transición de tema y tamaño óptico

- El cambio claro/oscuro anima color, fondo y borde durante 460 ms en los elementos afectados, sin imponer una transición global que interrumpa otras animaciones.
- Las dos variantes del personaje comparten marco; se funden entre sí. La variante blanca usa escala óptica de 108 % para igualar el tamaño percibido de la versión oscura.
- Esta decisión sustituye la conmutación inmediata de archivos del retrato.

## 9 de noviembre de 2026 — Primera landing del portafolio

- Se convirtió la arquitectura vigente a `CV.md` y se construyó `index.html` con el orden Inicio, Proyectos, Sobre mí y Contacto.
- Los siete proyectos aparecen en tres áreas. Las portadas son tipográficas y se identifican como provisionales hasta recibir las imágenes reales. No se inventaron años ni vínculos a casos todavía inexistentes.
- La apertura es tipográfica; el personaje permanece en Sobre mí. Instagram se muestra como usuario sin enlace hasta verificar la dirección del perfil.
- El sitio usa los tokens y fuentes del sistema, tema claro y oscuro, navegación móvil, foco visible y movimiento reducido.

## 9 de noviembre de 2026 — Carruseles de proyecto provisionales

- La landing presenta cada proyecto en un módulo amplio con tres espacios: portada, aplicación y detalle. Se recorren horizontalmente por gesto, teclado o botones.
- Las formas usan radio de 20 px en el marco. El azul aparece en una vista de acento y el rosa en un indicador pequeño. La superficie de cristal se limita a navegación y una etiqueta de estado.
- Los espacios están rotulados como provisionales; no representan imágenes ni resultados del proyecto.
- La arquitectura, `CV.md`, `DESIGN.md` y la landing comparten esta decisión.

## 9 de noviembre de 2026 — Portada centrada y nuevo orden

- La presentación se centra en nombre, enfoque y personaje. La ilustración se muestra una sola vez en la portada.
- El orden pasa a Inicio, Sobre mí, Proyectos y Contacto. La navegación y las llamadas a la acción siguen ese recorrido.
- La arquitectura, `CV.md`, el sistema de diseño y la landing registran esta decisión.

## 9 de noviembre de 2026 — Proyecto con imagen principal y miniaturas

- El módulo de cada proyecto sitúa el texto a la izquierda y una vista principal grande a la derecha en escritorio; en móvil se apilan.
- Cuatro miniaturas superpuestas cambian la vista principal: portada, sistema, detalle y aplicación. Las vistas siguen rotuladas como provisionales.
- Esta composición sustituye el carrusel horizontal anterior. Los documentos de sistema y arquitectura se actualizan con la misma regla.

## 2026-11-12 · Personaje animado en portada

- La portada sustituye las ilustraciones estáticas por un ciclo de cinco segundos, automático, silencioso y sin controles. Se conserva una imagen fija para la preferencia de movimiento reducido y para carga inicial.
- El original `assets/yo.mov` se mantiene solo como fuente local. Para la web se generaron dos versiones H.264 ligeras, una por tema, con el mismo recorte y tamaño para evitar saltos al cambiar de tema.
- Se actualizaron `index.html`, `DESIGN.md`, `CV.md` y los documentos de Word de sistema de diseño y arquitectura para describir la misma decisión. La tarjeta personal de `design.html` permanece estática porque es una muestra del componente, no una segunda portada.

## 2026-11-13 · Portada clara y firma personal

- El portafolio y la guía visual quedan en una sola base clara; se retira el selector de tema. Los colores oscuros siguen disponibles para bloques puntuales.
- La entrada usa el logotipo vectorial del nombre, cuyo peso progresa de extraligero a negro, junto al personaje. La frase principal organiza la jerarquía y reserva azul para «idea» y rosa para «forma».
- La animación del personaje se entrega como PNG animado transparente, en bucle y sin sonido. La imagen fija aparece con movimiento reducido. El fondo transparente elimina el recuadro visible de los videos comprimidos.
- Se actualizaron la página, la guía visual, DESIGN.md, CV.md y ambos documentos de Word para describir la misma decisión.

## 2026-11-13 · Interacción tipográfica en la entrada

- El SVG de la frase sirve como referencia de composición. La versión web usa texto real para permitir cambio por palabra y conservar lectura adaptable.
- «Idea» y «forma» parten en DM Sans Light. Al pasar el cursor, una capa DM Sans Medium Italic aparece con fundido breve y toma el azul o el rosa. En pantallas táctiles los acentos se muestran sin depender de hover; con movimiento reducido no hay transición.


## 13 de noviembre de 2026 — Revisión de coherencia y publicación

- Consolidación de DESIGN.md, CV.md y ambos Word: base clara, portada reactiva, orden de secciones, galerías reales de Quest y TipoFilicko, movimiento, zoom y arrastre. Se eliminaron reglas antiguas contradictorias y se separaron componentes de reserva y casos futuros.
- Guía visual actualizada con blanco puro para tarjetas, 11 tonos y 16 roles, muestra de galería y explicación de interacciones actuales. Corrección de la referencia de JavaScript que interrumpía sus animaciones.
- Correcciones funcionales acotadas en la landing: menú móvil con estilo consistente, enlace de Instagram y control para pausar movimiento automático. Las miniaturas se detienen con foco de teclado. Se conserva la composición aprobada.
- Verificación local en Chrome: imágenes y enlaces internos sin fallos; cambio de vista y zoom en ambas galerías; movimiento de miniaturas, pausa, menú a 390 px y movimiento reducido. Sin errores de JavaScript. Word renderizados y revisados visualmente. No constituye una auditoría completa de WCAG ni una prueba física en todos los dispositivos.
- Pendiente para entrega final: piezas de cinco proyectos, explicaciones de proceso, participación y créditos.
