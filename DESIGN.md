---
version: alpha
name: Aldo Iván — Sistema de diseño del portafolio
description: Portafolio claro de composición editorial, tipografía variable y acentos azules.
colors:
  primary: "#0C0C0C"
  on-primary: "#F4F4F4"
  secondary: "#4F4F4F"
  tertiary: "#105EF9"
  on-tertiary: "#F4F4F4"
  surface: "#F4F4F4"
  surface-card: "#FFFFFF"
  on-surface: "#0C0C0C"
  accent-graphic: "#0000F4"
typography:
  hero-name:
    fontFamily: DM Sans
    fontSize: 124px
    fontWeight: 200
    lineHeight: 118px
    letterSpacing: -6px
  hero-statement:
    fontFamily: DM Sans
    fontSize: 70px
    fontWeight: 300
    lineHeight: 74px
    letterSpacing: -2.8px
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
    letterSpacing: 0px
  meta:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
    letterSpacing: 0px
spacing:
  base: 4px
  xs: 8px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  section-mobile: 56px
  section-tablet: 72px
  section: 96px
  margin-mobile: 20px
  margin-tablet: 32px
  margin: 48px
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
---

## Overview

Este sistema describe la versión publicada del portafolio. El recorrido es portada, Sobre mí, índice de áreas, seis proyectos y contacto. La base es clara; Contenido y el pie usan negro. El personaje, la firma tipográfica y las piezas de cada proyecto dan identidad a la página.

## Colors

La página usa {colors.surface} como fondo, {colors.primary} para lectura principal y {colors.secondary} para texto secundario. Los marcos de proyectos y las tarjetas de marcas son blanco puro {colors.surface-card}. Contenido y el pie usan {colors.primary} con {colors.on-primary}. El azul {colors.tertiary} señala enlaces, estados de foco y las palabras «idea» y «forma»; {colors.accent-graphic} colorea las tres cintas divisorias. Los colores propios de los proyectos aparecen dentro de sus imágenes y no son nuevos colores de la interfaz. La identidad del portafolio no usa rosa.

El texto principal sobre fondo claro y el texto claro sobre negro superan WCAG AA. El azul de acción sobre {colors.surface} ofrece aproximadamente 4.78:1. Los enlaces sobre negro se muestran claros y subrayados.

## Typography

DM Sans variable construye nombre, titulares, navegación y controles; Manrope variable sostiene los párrafos y metadatos. Ambas fuentes se sirven localmente en WOFF2. La firma «aldo iván» comienza en peso 200. Durante la primera interacción cada letra se acerca a un peso progresivo, de 200 a 900; al salir el cursor se transforma en el mismo logotipo vectorial de la cabecera y ya no repite el efecto. La frase «me gusta entender una idea antes de darle forma» reacciona por letra a la proximidad del cursor, manteniendo cada fila independiente. «idea» y «forma» comparten azul.

Los títulos de sección como «Sobre mí» y «Contenido» comparten jerarquía DM Sans 700. Los nombres de proyectos usan 56/58 px en escritorio y se reducen en móvil. Los tamaños de la portada son fluidos para caber en la altura visible.

## Layout

El contenedor mide como máximo 1296 px, incluidos sus márgenes internos. El margen lateral es de 20 px en móvil, 32 px en tableta y 48 px desde 1024 px. Los proyectos tienen texto a la izquierda e imagen a la derecha en escritorio, con proporción aproximada 42/58; bajo 1024 px pasan a una columna. Sobre mí alinea su texto con el margen general y coloca un ojo decorativo a la derecha. El índice de áreas y los divisores ocupan todo el ancho. Las miniaturas llegan al borde izquierdo de la pantalla sin provocar desplazamiento horizontal de la página.

## Elevation & Depth

La profundidad proviene del contraste entre fondo claro, tarjetas blancas y bandas negras. Las tarjetas no llevan sombras permanentes ni efecto cristal. Solo la cabecera usa una superficie clara translúcida con desenfoque de 16 px para mantener legibilidad al desplazarse; los controles circulares de galería tienen una sombra ligera. Las secciones entran con un fundido y desplazamiento corto al cruzar el área visible.

Las cintas «branding», «campañas» y «motion graphics» avanzan continuamente de derecha a izquierda. Sus letras aumentan de peso y tamaño según la cercanía del cursor. El índice y las miniaturas también avanzan automáticamente y aceptan interacción manual; Pausar y la preferencia de movimiento reducido detienen los ciclos.

## Shapes

Los marcos de imágenes, miniaturas y videos usan {rounded.xl}. Las tarjetas de marcas son blancas y de esquinas redondeadas; no llevan contorno. Los controles de galería son círculos de 38 px. El personaje de portada aparece sin recuadro. El material visual de cada proyecto conserva su color original.

## Components

**Portada.** Personaje animado arriba, firma «aldo iván», rótulo «diseñador gráfico» y frase en tres líneas. La firma pasa una sola vez al logo vectorial. En móvil se ajustan los tamaños para conservar la composición.

**Índice de áreas.** Tres tarjetas enlazan Branding, Campañas y Motion Graphics y se mueven horizontalmente. El trackpad permite recorrerlas manualmente.

**Divisores.** Branding presenta Quest y TipoFilicko; Campañas presenta Macabro y movo; Motion Graphics solo muestra la cinta de texto. Las tres cintas usan el mismo movimiento y reacción tipográfica.

**Galerías.** Quest, TipoFilicko, Macabro y movo empiezan con su logo. Miniaturas, flechas y trackpad cambian la imagen principal. Los mockups se pueden ampliar y arrastrar sin cambiar la forma del marco. Las miniaturas muestran fragmentos de las vistas siguientes y avanzan hacia la izquierda.

**Videos.** Tipognoma y Robot Dreams muestran un video 16:9 cada uno, completo dentro de un marco redondeado y con controles de reproducción y sonido.

**Contacto.** El pie negro reúne Instagram @alivaan__, el correo alditto172@gmail.com, regreso al inicio y un ojo pequeño abajo a la derecha. Los enlaces mantienen foco visible.

## Do's and Don'ts

- Mantener el orden narrativo y la lectura accesible en móvil y escritorio.
- Usar azul para interacción y acentos de texto; conservar los colores originales dentro de las piezas de proyecto.
- Identificar las propuestas académicas y la participación individual; no atribuir encargos o resultados no comprobados.
- Permitir pausa y movimiento reducido sin perder contenido ni navegación.
- Evitar rosa, cristal en tarjetas, sombras decorativas, nuevos modos de color y componentes ajenos al portafolio.
