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
  surface-card: "#FFFFFF"
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
  hero-name:
    fontFamily: DM Sans
    fontSize: 106px
    fontWeight: 200
    lineHeight: 101px
    letterSpacing: -5.3px
  project-title:
    fontFamily: DM Sans
    fontSize: 56px
    fontWeight: 700
    lineHeight: 58px
    letterSpacing: -1px
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
    fontSize: 70px
    fontWeight: 300
    lineHeight: 74.2px
    letterSpacing: -2.8px
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
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.primary}"
    typography: "{typography.project-title}"
    rounded: "{rounded.xl}"
  link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.tertiary}"
    typography: "{typography.body}"
  modal:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.xl}"
  gallery-control:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    size: 38px
---

## Overview

Mi portafolio presenta mi trabajo como estudiante de diseño gráfico mediante una composición editorial de base clara, una firma tipográfica sensible al cursor y proyectos con imagen dominante. La personalidad está en la relación entre tipografía, personaje y piezas reales, no en acumular efectos. La versión vigente se revisó el 13 de noviembre de 2026.

El recorrido es portada, índice de áreas, Sobre mí, proyectos agrupados y contacto. El índice facilita el acceso directo; Sobre mí aporta contexto antes de revisar el trabajo. No hay selector de tema. La guía visual distingue las reglas del portafolio de los componentes de reserva que todavía no se utilizan.

## Colors

El fondo es {colors.surface}, la lectura principal {colors.primary} y la secundaria {colors.secondary}. Las tarjetas y el marco de galería usan blanco puro {colors.surface-card}; esa diferencia respecto al fondo delimita los planos sin contornos ni sombras permanentes. El índice de áreas usa {colors.primary} como banda oscura, con tarjetas claras. La franja de marcas conserva el fondo claro.

{colors.tertiary} identifica navegación y acentos de interacción. {colors.accent-graphic} aparece en la cinta «branding» y en recursos gráficos; {colors.accent-detail} destaca «forma». En la frase se admiten azul y rosa porque distinguen idea y realización, sin crear dos acciones de navegación. Los colores de Quest y TipoFilicko pertenecen a esos proyectos y no amplían la paleta de la marca personal.

Los 16 roles cromáticos corresponden a 11 valores únicos. Los alias on-primary, on-tertiary y on-surface-dark comparten #F4F4F4; on-surface comparte #0C0C0C y on-surface-muted comparte #222222. La guía agrupa los valores repetidos. Surface-dark, surface-raised, surface-muted y text-muted-dark sirven para muestras y estados de componentes, no implican un modo oscuro.

Sobre #F4F4F4, #0C0C0C ofrece 17.79:1, #4F4F4F 7.45:1 y #105EF9 4.78:1. El rosa #EF1889 ofrece aproximadamente 3.70:1: se limita a texto grande o detalles sin información esencial. Sobre oscuro, los enlaces pequeños deben ser claros y subrayados. Una revisión de estos pares no equivale a una certificación de accesibilidad de toda la página.

## Typography

DM Sans variable construye nombre, titulares y controles; Manrope variable sostiene párrafos y metadatos. Se cargan localmente en WOFF2. DM Sans permite pesos 100–1000 y Manrope 200–800. No se usa cursiva en las interacciones actuales.

El nombre «aldo iván» está en minúsculas y peso 200 en reposo. Cada letra responde a la proximidad del cursor; sus pesos máximos progresan 200, 300, 400, 500, 600, 700, 800 y 900. La primera «a» conserva su peso pero participa en color y escala. El crecimiento máximo es 12 % y el desplazamiento vertical 3 px, sin cambiar los espacios reservados. El logotipo vectorial permanece en la navegación; la portada emplea texto real.

La frase «me gusta entender una idea antes de darle forma», sin punto final, parte de peso 300. Solo reacciona la fila más cercana al cursor; «idea» y «forma» pueden alcanzar peso 700 y sus acentos azul y rosa. La escala máxima es 6 % y el desplazamiento 0.8 px. El peso y el color se interpolan suavemente. En pantallas táctiles los acentos se muestran sin exigir hover.

La escala base de la guía conserva apertura 80/80, sección 48/52, subtítulo 20/26, cuerpo 18/28, navegación 16/20, metadatos 14/20 y notas 12/16 px. No todos estos ejemplos son titulares de la landing. El título de proyecto usa 56/58 px en escritorio y escala desde 32 px en móvil. Los rótulos de grupo usan 28/32 px.

La portada tiene tamaños fluidos para aprovechar la altura: el nombre alcanza 106 px y la frase 70 px; en móvil el nombre varía entre 52 y 78 px y la frase entre 30 y 48 px. El interletrado del nombre es −0.05 em y el de la frase −0.04 em. Estos ajustes propios de portada se distinguen de la escala base; no se afirma que toda pantalla use tamaños fijos. Con zoom de lectura se permite desplazamiento vertical antes que recortar contenido.

## Layout

El contenedor del portafolio mide como máximo 1296 px incluyendo márgenes internos. Desde 1024 px los márgenes son 48 px: el contenido útil máximo es 1200 px. Por debajo de 600 px son 20 px; entre 600 y 1023 px, 32 px. La separación general entre secciones es 56, 72 y 96 px respectivamente. La base de espaciado es 4 px, con ajustes locales de 10 y 14 px en las miniaturas.

Las 12 columnas de la guía son una referencia editorial, no doce columnas obligatorias en todos los componentes. Los proyectos usan dos zonas proporcionales 42/58 en escritorio, separadas 32 px; por debajo de 1024 px pasan a una columna, con texto antes de la galería. La portada centra verticalmente personaje, nombre, profesión y frase. El índice y la cinta de marcas se extienden a todo el ancho.

La imagen principal está a la derecha y la tira de miniaturas se superpone desde la izquierda en la parte baja. Su soporte opaco, del color del fondo, genera el hueco entre planos; no es cristal ni transparencia. Se ven aproximadamente tres miniaturas y fragmentos de las siguientes durante el movimiento. En móvil la tira queda al pie de la imagen. Los marcos mantienen su geometría cuando cambia el contenido.

## Elevation & Depth

El cristal se reserva a la cabecera: superficie clara al 88 % y desenfoque de 16 px. Las galerías y miniaturas son sólidas. Las flechas y controles de zoom son círculos blancos con una sombra ligera de 0 2px 12px y negro al 12.5 %. Las tarjetas no llevan sombra permanente.

La entrada de secciones combina 28 px de desplazamiento y un fundido de 550 ms, repetido al volver a entrar. El índice de áreas se mueve en bucle hacia la izquierda en ciclos de 20 s; al señalar una tarjeta baja al 40 % de velocidad y desenfoca las demás. Las cintas «branding» y «campañas» se desplazan aproximadamente 75 px/s. Las miniaturas avanzan 85 px/s y bajan a 45 px/s bajo el cursor; el gesto horizontal permite acelerar o retroceder. El foco de teclado detiene la tira de miniaturas.

El cambio de imagen real usa un fundido de 380 ms, con la imagen entrante ya ajustada al marco. El zoom interpola únicamente la transformación durante 240 ms; el arrastre es directo para evitar retrasos. El control Pausar detiene las cintas, las miniaturas y sustituye el personaje por su imagen fija. La preferencia de movimiento reducido elimina los ciclos y transiciones y mantiene el acceso manual.

## Shapes

Las galerías y miniaturas usan {rounded.xl}, 20 px, sin stroke. El logo inicial aparece completo, centrado, al 70 % del marco y ligeramente elevado; los mockups llenan el marco y pueden recorrerse mediante arrastre. El recorte nunca se presenta como una imagen completa.

Botones generales usan 12 px, muestras de navegación flotante 16 px y controles de galería una forma circular de 38 px. Las tarjetas vectoriales del índice conservan su forma original; no deben recortarse para simular una geometría distinta. El personaje no lleva marco.

## Components

**Portada.** Personaje animado transparente arriba; nombre reactivo debajo; rótulo «diseñador gráfico» y frase en tres líneas. No tiene botones de llamada a la acción ni párrafo adicional. La condición de estudiante se explica en Sobre mí.

**Navegación.** Enlaces al inicio, Sobre mí, Proyectos y Contacto. En móvil, un botón Menú abre los mismos destinos. Pausar permite detener el movimiento automático. El foco debe ser visible; los enlaces siguen funcionando sin depender del efecto del cursor.

**Índice de áreas.** Tres tarjetas enlazan Branding, Campañas y Motion Graphics. Sus copias permiten continuidad visual y se excluyen del orden de tabulación. El gesto horizontal no debe bloquear el desplazamiento vertical de la página.

**Franja de marcas.** Quest y TipoFilicko enlazan a sus módulos de identidad. Antes del grupo de campañas, Macabro y movo enlazan a sus proyectos. Detrás de cada grupo circula «branding» o «campañas» en azul gráfico; un desvanecido del color de fondo de 25 px alrededor del grupo evita que compita con los logotipos. Los recuadros son blancos y sin contorno.

**Galería de proyecto.** Nombre, categoría, descripción y alcance acompañan una imagen grande. Quest comienza con su logotipo y tiene cinco mockups; TipoFilicko comienza con su logotipo y tiene nueve; MACABRO FICH comienza con el logotipo entregado y tiene cinco imágenes; movo comienza con su logotipo y tiene cinco imágenes. Las miniaturas, las flechas y el gesto horizontal cambian la imagen. Los mockups admiten zoom de 1 a 2.5 en pasos de 0.25, centrado en la posición reciente del cursor, y arrastre limitado a los bordes. El logo no se amplía. Al cambiar de imagen se restablece el encuadre. Las flechas del teclado permiten desplazar el mockup cuando tiene foco.

**Contenido pendiente.** movo, Tipognoma y Robot Dreams conservan vistas provisionales. No existen páginas de caso separadas ni resultados documentados en ellas. Se incorporarán piezas, explicaciones de participación y créditos cuando estén disponibles.

**Contacto.** Enlace a Instagram @alivann y retorno al inicio. No hay formulario de envío. Botones generales, campos, etiquetas y modal de la guía son ejemplos de reserva; no se presentan como funciones activas del portafolio.

## Do's and Don'ts

- Mantener el mismo orden narrativo en móvil y escritorio; permitir lectura y navegación sin hover.
- Conservar el color original de cada proyecto y distinguir propuestas conceptuales de encargos oficiales.
- Mantener blancos sólidos, radios de 20 px y encuadres estables durante las transiciones.
- Usar el movimiento para orientar y explorar, con pausa y alternativa reducida; no añadir más efectos a las galerías.
- No sustituir explicaciones de concepto, participación y créditos por mockups. Las galerías muestran ejecución, pero todavía no constituyen casos completos.
- No usar rosa en texto pequeño sobre claro ni azul de acción en texto pequeño sobre oscuro.
- No describir componentes de reserva o páginas futuras como prestaciones ya publicadas.
