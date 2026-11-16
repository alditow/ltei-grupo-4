# Sistema de diseño de Aldo Iván

## 1 · Personalidad y propósito

Mi sistema visual parte de una idea sencilla: entender antes de dar forma. Por eso combina una composición editorial clara con elementos que invitan a explorar. La tipografía establece la jerarquía, el espacio permite distinguir cada parte y el movimiento señala que hay más contenido por descubrir.

La página comienza con una presentación centrada. Después, la información se organiza en Sobre mí, un índice de áreas, los trabajos y el contacto. Esta secuencia permite conocer primero mi manera de pensar y luego recorrer lo que hago.

La interfaz mantiene una identidad constante. Cada trabajo puede mostrar sus propios colores dentro de sus imágenes, pero esos colores no sustituyen la paleta del portafolio.

## 2 · Colores

La paleta de la interfaz es breve y cada color tiene una función.

- Gris claro — #F4F4F4. Es el fondo general. Su tono suave permite que las tarjetas blancas se distingan sin necesidad de bordes.

- Blanco — #FFFFFF. Se reserva para tarjetas, marcos de imagen y controles situados sobre las imágenes.

- Negro — #0C0C0C. Es el color del texto principal. También construye la franja de contenido y el pie de página.

- Blanco de lectura — #F4F4F4. Se utiliza para texto sobre las superficies negras.

- Gris medio — #4F4F4F. Identifica descripciones y datos secundarios sin perder legibilidad.

- Azul de interacción — #105EF9. Señala enlaces, etiquetas de área, foco de teclado y palabras destacadas de la presentación.

- Azul gráfico — #0000F4. Se reserva para las cintas de texto que separan las áreas del trabajo.

El azul tiene un papel preciso: guiar la atención y mostrar interacción. No se aplica a grandes superficies ni se combina con otros acentos de la interfaz. Para texto normal, las combinaciones previstas alcanzan el contraste mínimo de accesibilidad de 4.5:1.

## 3 · Tipografía

Uso dos familias variables con funciones distintas. DM Sans da carácter a la firma, los títulos, la navegación y los controles. Manrope sostiene los párrafos, las descripciones y los datos breves. Ambas se usan en formato web WOFF2.

La firma «aldo iván» comienza en DM Sans ExtraLight. Su ligereza permite que el cambio de peso de cada letra sea parte de la identidad. La frase «me gusta entender una idea antes de darle forma» mantiene una apariencia ligera y ocupa tres líneas en la portada. El oficio, «diseñador gráfico», funciona como un rótulo más pequeño entre ambos elementos.

Esta es la escala de referencia en escritorio:

- Firma: hasta 124 px, peso inicial 200, interlineado de 0.95 e interletrado de −0.05 em.

- Frase de presentación: hasta 70 px, peso 300, interlineado de 1 e interletrado de −0.04 em.

- Título de sección: 48 px con interlineado de 52 px y peso 700.

- Título de trabajo: 56 px con interlineado de 58 px y peso 700.

- Texto de lectura: Manrope de 16 px con interlineado de 25 px.

- Navegación: DM Sans de 16 px con interlineado de 20 px y peso 500.

- Datos secundarios: Manrope de 14 px con interlineado de 20 px.

En móvil, la firma y la frase reducen su tamaño según el ancho y la altura disponibles. Los títulos de sección pasan a 32/36 px y los de trabajo comienzan en 32 px. El texto esencial conserva un tamaño cómodo de lectura; las notas de 12 px no contienen información indispensable.

## 4 · Layout y espaciado

La composición se construye a partir de una unidad de 4 px. Los espacios de uso frecuente son 8, 12, 16, 24 y 32 px. Las separaciones entre secciones son mayores para que el recorrido tenga pausas claras: 56 px en móvil, 72 px en tableta y 96 px en escritorio.

El contenido tiene un ancho máximo de 1296 px, incluidos sus márgenes interiores. Los márgenes laterales son de 20 px en móvil, 32 px en tableta y 48 px en escritorio. Esta medida mantiene alineados títulos, párrafos y controles sin impedir que algunas piezas ocupen todo el ancho de la pantalla.

La portada es la excepción deliberada a la alineación lateral: personaje, firma, oficio y frase forman una composición centrada dentro de la primera pantalla. A partir de Sobre mí, la lectura vuelve al margen izquierdo.

Los trabajos usan una composición de dos zonas en escritorio: aproximadamente 42 % para la información y 58 % para la imagen principal. Una tira horizontal de vistas pequeñas cruza la parte inferior y se extiende hacia el margen izquierdo. En pantallas estrechas, texto e imagen se apilan en una columna. La página no debe producir desplazamiento horizontal accidental; solo las tiras previstas se recorren lateralmente.

## 5 · Profundidad

La profundidad proviene principalmente de la relación entre superficies: fondo gris claro, tarjetas blancas y franjas negras. Los marcos de los trabajos son sólidos y dejan que las imágenes tengan protagonismo.

La cabecera utiliza una transparencia discreta y un desenfoque de 16 px para conservar su lectura mientras la página se desplaza. Los controles sobre imágenes pueden tener una sombra leve que los separe del contenido. Las sombras de las tarjetas aparecen de forma puntual durante una interacción; no son una capa decorativa permanente.

## 6 · Formas

Las tarjetas, los marcos grandes y las miniaturas comparten esquinas redondeadas de 20 px. Mantener el mismo radio hace que una vista pequeña y su versión ampliada se perciban como partes de un mismo componente.

Los controles de galería son círculos blancos de 38 px. El personaje de la portada aparece libre sobre el fondo, sin tarjeta ni contorno. Las imágenes ocupan su marco sin deformarse: cuando un recorte oculta detalles, la persona puede ampliar y desplazar la imagen dentro de ese mismo espacio.

## 7 · Componentes

Cabecera. El logotipo se sitúa a la izquierda y los enlaces principales quedan centrados en escritorio. En móvil, la navegación se adapta al espacio disponible. Los enlaces muestran un foco visible al navegar con teclado.

Portada. El personaje, la firma, el oficio y la frase forman una sola jerarquía. Cada elemento tiene una función: identificarme, decir qué hago y expresar mi manera de trabajar.

Índice de áreas. Tres tarjetas permiten entrar a las áreas del portafolio. Se presentan sobre una franja negra y se desplazan horizontalmente. La interacción permite recorrerlas también de forma manual.

Divisores de área. Una cinta de texto azul cruza todo el ancho de la pantalla antes de cada grupo de trabajos. Su repetición y movimiento anuncian un cambio de sección sin añadir un título estático redundante.

Presentación de trabajos. Cada bloque reúne área y número, título, descripción breve y alcance. La imagen principal ocupa un marco blanco a la derecha; las miniaturas se superponen a su parte inferior y permiten elegir otra vista. Las flechas y el desplazamiento horizontal ofrecen formas adicionales de recorrerlas. El cambio de vista conserva el tamaño y las esquinas del marco.

Contacto. Un pie negro reúne la invitación a conversar, los enlaces de Instagram y correo, el regreso al inicio y un ojo pequeño en la esquina inferior derecha.

## 8 · Movimiento e interacción

El movimiento forma parte de la identidad porque acompaña la exploración; no sustituye el contenido.

La firma responde letra por letra a la proximidad del cursor. Parte de ExtraLight y cada carácter puede adquirir un peso progresivamente mayor, desde la primera «a» hasta la última «n». Al alejarse el cursor, vuelve suavemente a su estado inicial y puede reaccionar otra vez. En la frase de presentación, el efecto se limita a la línea próxima; «idea» y «forma» incorporan el azul de interacción.

Las cintas de las áreas avanzan continuamente de derecha a izquierda. Sus letras también reaccionan de forma individual al cursor, cambiando de tamaño y peso sin desplazar la composición. El texto permanece azul durante la interacción.

Las tarjetas del índice y las miniaturas avanzan de forma continua, pero también se pueden recorrer con el trackpad. Al seleccionar una miniatura, la nueva vista aparece mediante una transición suave, sin estirar la imagen. Las secciones entran con un desplazamiento y un fundido breves cada vez que vuelven al área visible.

Cuando el dispositivo solicita menos movimiento, los ciclos automáticos se detienen y permanecen disponibles las acciones manuales.

## 9 · Comportamiento responsivo

El diseño parte de una columna en móvil y gana amplitud de forma gradual. Por debajo de 600 px utiliza márgenes de 20 px; desde 600 px, de 32 px; y desde 1024 px, de 48 px.

En móvil se reducen la firma y la frase para que la portada siga siendo una composición completa. Los trabajos pasan de dos zonas a una columna. Las miniaturas continúan siendo una tira horizontal independiente, accesible al tacto. En escritorio, la relación entre texto, imagen grande y vistas pequeñas recupera la composición amplia.

Los controles deben conservar un foco visible y un nombre comprensible. El contenido y la navegación siguen disponibles aunque una animación esté detenida.

## 10 · Reglas de uso

**Sí**

- Usa la jerarquía tipográfica para ordenar la lectura antes de añadir recursos decorativos.

- Mantén el gris claro como base, el blanco para tarjetas y el negro para las franjas de contraste.

- Reserva el azul para interacción, señales de recorrido y acentos tipográficos.

- Conserva el radio de 20 px entre imagen grande, miniaturas y tarjetas.

- Permite recorrer las galerías con controles, teclado y desplazamiento horizontal.

- Explica cada trabajo con textos breves que dejen espacio a sus imágenes.

- Asegura que el contenido siga siendo legible y utilizable con movimiento reducido.

**No**

- Añadas colores de un trabajo a la interfaz general.

- Uses sombras, transparencias o desenfoques como decoración de todas las tarjetas.

- Estires una imagen para obligarla a llenar un marco.

- Cambies el radio o las proporciones de un componente entre sus estados.

- Coloques varios acentos compitiendo dentro de una misma zona.

- Uses animaciones que impidan leer, elegir una vista o controlar el recorrido.

- Dependás únicamente del color para comunicar que algo se puede activar.
