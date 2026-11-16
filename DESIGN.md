---
version: "2.0"
name: Aldo Iván — Sistema de diseño
summary: Composición editorial clara, tipografía variable y movimiento que guía la exploración.
colors:
  primary: "#0C0C0C"
  on-primary: "#F4F4F4"
  secondary: "#4F4F4F"
  surface: "#F4F4F4"
  surface-card: "#FFFFFF"
  on-surface: "{colors.primary}"
  tertiary: "#105EF9"
  on-tertiary: "#F4F4F4"
  accent-graphic: "#0000F4"
typography:
  hero-name:
    fontFamily: DM Sans
    fontSize: 106px
    fontWeight: 200
    lineHeight: 0.95
    letterSpacing: "-0.05em"
  hero-statement:
    fontFamily: DM Sans
    fontSize: 70px
    fontWeight: 300
    lineHeight: 1
    letterSpacing: "-0.04em"
  section:
    fontFamily: DM Sans
    fontSize: 48px
    fontWeight: 700
    lineHeight: 52px
    letterSpacing: -1px
  project-title:
    fontFamily: DM Sans
    fontSize: 56px
    fontWeight: 700
    lineHeight: 58px
    letterSpacing: -1px
  body:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: 400
    lineHeight: 25px
  navigation:
    fontFamily: DM Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 20px
  meta:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
spacing:
  base: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  section-mobile: 56px
  section-tablet: 72px
  section-desktop: 96px
  margin-mobile: 20px
  margin-tablet: 32px
  margin-desktop: 48px
rounded:
  sm: 4px
  md: 12px
  lg: 16px
  xl: 20px
  full: 9999px
components:
  page:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
  dark-band:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  card:
    backgroundColor: "{colors.surface-card}"
    rounded: "{rounded.xl}"
  gallery-control:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.primary}"
    rounded: "{rounded.full}"
    size: 38px
  focus:
    color: "{colors.tertiary}"
    width: 3px
---

## Overview

La identidad parte de observar, comprender y dar forma. La composición editorial mantiene una lectura clara; la tipografía variable aporta personalidad y el movimiento indica que hay más contenido por explorar. El recorrido del portafolio es presentación centrada, Sobre mí, índice de áreas, trabajos y contacto. Solo existe tema claro. Las obras mantienen sus propios colores dentro de sus imágenes; la interfaz conserva su paleta.

## Colors

{colors.surface} cubre la página. {colors.surface-card} separa tarjetas y marcos de imagen. {colors.primary} es tinta principal y fondo de la franja Contenido y del pie; {colors.on-primary} se usa sobre esas áreas. {colors.secondary} corresponde a lectura secundaria. {colors.tertiary} marca enlaces, foco, etiquetas y «idea» y «forma». {colors.accent-graphic} se reserva para el texto de las cintas divisorias. Un área no acumula varios acentos.

Los pares de lectura normal superan 4.5:1: primary/surface ≈17.8:1; secondary/surface ≈7.45:1; tertiary/surface ≈4.78:1; on-primary/primary ≈17.8:1. El color de las obras no se adopta como token de la interfaz. No hay rosa en la paleta vigente.

## Typography

DM Sans variable en WOFF2 construye firma, títulos, navegación y controles; Manrope variable en WOFF2 sostiene párrafos y metadatos. La firma comienza en peso 200 y cada letra reacciona a la cercanía del cursor hacia un peso propio progresivo de 200 a 900; vuelve a peso 200 al alejarse y puede repetirse. No se sustituye permanentemente por el logotipo. La frase «me gusta entender una idea antes de darle forma» tiene tres líneas; «idea» y «forma» son azules y reaccionan por letra y por línea sin mover la retícula.

Escala de referencia en escritorio: firma hasta 106 px con interlineado .95 y espaciado −.05em, ajustada también a la altura de pantalla; frase hasta 70 px con espaciado −.04em; sección 48/52 px, peso 700; título de trabajo 56/58 px, peso 700; cuerpo Manrope 16/25 px; navegación DM Sans 16/20 px, peso 500; metadatos Manrope 14/20 px. El rótulo «diseñador gráfico» es DM Sans 500 y crece hasta 20 px. En móvil la firma usa 52–78 px según altura disponible, la frase 30–48 px, los títulos de sección 32/36 px y los de trabajo parten de 32 px. El contenido esencial nunca se presenta en la nota de 12 px.

## Layout

El contenedor máximo mide 1296 px incluyendo sus márgenes internos. Los márgenes son 20 px bajo 600 px, 32 px desde 600 px y 48 px desde 1024 px. La separación principal entre secciones es de 56, 72 y 96 px en esos mismos rangos. La portada centra personaje sin marco, firma, oficio y frase dentro de la altura visible. Sobre mí alinea la lectura al margen y sitúa un ojo decorativo a la derecha.

El índice de áreas y los divisores se extienden a todo el ancho. Cada trabajo dispone texto a la izquierda y una imagen principal a la derecha, aproximadamente 42/58 en escritorio; bajo 1024 px pasa a una columna. Una tira horizontal de vistas pequeñas se superpone en el borde inferior de la composición sin dejar un hueco transparente. Las miniaturas pueden alcanzar el borde izquierdo de la pantalla; el documento no debe desplazarse horizontalmente. La selección muestra la imagen en el marco grande y conserva visibles las otras vistas.

## Elevation & Depth

La profundidad se construye con fondo gris claro, tarjetas blancas y franjas negras. Los marcos son superficies sólidas, sin cristal ni sombras permanentes. La cabecera translúcida usa desenfoque de 16 px para conservar legibilidad al desplazarse. Los controles circulares sobre imágenes admiten sombra leve; la tarjeta activa del índice gana una sombra temporal para distinguir el primer plano. Las secciones aparecen con un desplazamiento y fundido corto al entrar en el área visible, y repiten la reacción al volver a entrar.

### Composición y movimiento

Las cintas «branding», «campañas» y «motion graphics» cruzan el ancho completo y avanzan de derecha a izquierda en ciclo continuo. Las letras aumentan suavemente su peso y tamaño según la distancia al cursor sin alterar la posición de las demás. La firma y la frase también reaccionan letra por letra; la frase limita el efecto a la línea próxima. El índice de áreas y las miniaturas se desplazan automáticamente y admiten recorrido manual con trackpad. El foco y la interacción detienen o ralentizan el índice y las miniaturas cuando corresponde; las cintas siguen avanzando mientras reaccionan al cursor. La preferencia del sistema por movimiento reducido detiene los ciclos y deja accesibles las opciones manuales. La cabecera no muestra un botón de pausa.

## Shapes

Los marcos grandes de imagen, las miniaturas y las tarjetas usan {rounded.xl}, equivalente a 20 px. Los controles de galería son círculos de 38 px con {rounded.full}; los estados deshabilitados mantienen su forma. El personaje de portada no tiene recuadro. Las imágenes llenan el marco; cuando el recorte deja fuera contenido, el usuario puede ampliar y arrastrar la imagen dentro del mismo marco. Las tarjetas no cambian de radio entre estados.

## Components

**Cabecera.** Logotipo a la izquierda, tres enlaces centrados horizontal y verticalmente en escritorio y menú accesible en móvil. El foco es visible. No hay botón «Pausar».

**Portada.** Personaje, firma, oficio y frase forman una composición centrada. El personaje usa una secuencia visual y una imagen fija cuando se reduce el movimiento. La firma vuelve a reaccionar en cada entrada del cursor.

**Índice y divisores.** Tres tarjetas enlazan las áreas. La franja Contenido es negra; los divisores de área tienen texto azul en movimiento sobre fondo claro. El área de movimiento usa solo su cinta de texto.

**Presentación de trabajos.** Un bloque de texto contiene área, número, título, descripción y alcance. A la derecha domina un marco blanco de imagen; una tira de miniaturas se superpone abajo y sale hacia el margen izquierdo. No se añaden contornos. La primera vista es el logo en trabajos de identidad o campaña. Flechas, miniaturas y trackpad cambian la vista; zoom y arrastre permiten inspeccionar detalles. La transición entre vistas no deforma la imagen ni el marco. Los trabajos de movimiento usan un marco de reproducción 16:9 con controles.

**Contacto.** El pie negro reúne invitación a conversar, Instagram, correo, regreso al inicio y un ojo pequeño en la esquina inferior derecha. Los enlaces tienen nombre accesible y foco visible.

## Do's and Don'ts

**Sí:** mantener la secuencia narrativa y la retícula; usar azul para interacción y acentos medidos; conservar el color propio dentro de cada obra; respetar los radios y el espacio entre marcos; permitir navegación por teclado, trackpad y movimiento reducido; distinguir con honestidad las propuestas académicas y la colaboración.

**No:** añadir colores a la interfaz por decoración; usar cristal o sombras en tarjetas; estirar imágenes; cambiar tamaños o radios de una tarjeta al interactuar; usar movimiento que impida leer o elegir; confiar solo en color para indicar una acción; describir un control que no existe en la página.
