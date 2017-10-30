# FREELANCER

* **Track:** _Common Core_
* **Curso:** _Creando tu primer sitio web interactivo_
* **Unidad:** _Maquetado web con HTML & CSS_

***
## Descripción
Se muestra el replicado, solo maquetación, de la página web **freelancer** (la imagen se muestra en la parte inferior "imagen usado para el replicado")para ello se creo una archivo **index.html** el cual contiene: un _HEADER_ , _SECTION 1 (Start bootstrap)_ , _SECTION 2 (Portfolio)_ , _SECTION 3 (About)_ , _SECTION 4 (contact)_ , _FOOTER_; un archivo **maincss** para darle los estilos correspondientes en las cuales figuran propiedades como: _position fixed_ para header, _position float_ para footer, _Display inline-block_ para las imagenes de la section 2 portafolio y las columnas de texto de section 3, _position relative_ , etc.

## Pseudocódigo (main.CSS)

- SETEAR NUESTROS ARCHIVOS para que sea igual para todos los navegadores para ello se agrega estilos a _BODY_.

  BODY:

    - Aplicar box-sizing:border-box; (para que se respete el ancho de las cajas)
    - Aplicar tipo de letra: _lato_;
    - Aplicar alto de línea: 1.5;
    - Aplicar margen y relleno: 0;

- ESTILOS AL **ENCABEZADO**:

  <HEADER></HEADER>:

    - Aplicar color de fondo negro (#2c3e50);
    - Aplicar tipo de letra: _Montserrat_;
    - Aplicar grosor de letra: 700; Escribir margen: 0;
    - Posicionar fijamente(**fixed**) con posicion parte superior cero;
    - Transfromar el texto a Mayuscula;
    - Aplicar un ancho de 100% para que ocupe todo el ancho de la página;
    - Aplicar un Z-index 1000 para que se superponga a la section 1;

  <NAV> </NAV> (hijo de HEADER):

    - Aplicar margen cero y un ancho de 95.6% con respecto a su padre HEADER;

  <DIV></DIV> (hijos de NAV):

    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block);
    - Aplicar un ancho de 49.5% conrespecto a NAV (su padre);

  <li></li>( hijo de ul y nieto de DIV)(barra de menú):

    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block);
    - Aplicar tamaño de letra 17px, espacio entre cada letra de 1px;
    - Posicionar en forma "relative" un 33% a la derecha respecto a su posicion actual;
    - Aplicar un margen y relleno cero;
    - Aplicar una pseudoclase: **hover** con color de letra: #18bc9c;
    - Aplicar una pseudoclase: **focus** con color de fondo: #18bc9c y color de letra blanco;

  <A></A>(links, hijos de li):
    - Aplicar un borde tipo radio de 4px;
    - Aplicar un color blanco (#fff) y quitar el subrayado;
    - Aplicar un margen cero;
    - Aplicar un relleno superior e inferior de 14px, izquierdo y derecho de 7px para separar las palabras entre si;

   <A ID=BOOTSTRAP></A>(hijo de DIV y nieto de NAV)
    - Posicionar en forma "relative" un 29% a la derecha respecto de su posición actual;
    - aplicar un tamaño de letra 1.5 em;

- ESTILOS GENERALES EN COMUN PARA LAS SECCIONES 1(START BOOTSTRAP),2(PORTFOLIO),3(ABOUT) Y 4(CONTACT ME); Y PIE DE PÁGINA(FOOTER):
   <SECTION></SECTION>:
    - Aplicar un margen de cero y un relleno superior e inferior de 100px;
    - Aplicar un ancho de 100% para que ocupe todo el ancho de página;

   <H1, H2, H3, H4></H1, H2, H3, H4>:
    - Aplicar margen cero;

   <DIV. CONTAINER></DIV>(hijos de los sections)
    - Aplicar margen izquierdo de 23px, un relleno de 15px  y un ancho de 95% respecto a sus padres sections;
    - Alinear los contenidos al centro;

   <IMG>:
    - Alinear verticalmento hacia el medio (vertical align);

- ESTILOS PARA LAS SECCIONES 1(START BOOTSTRAP) y 3(ABOUT) QUE CONTIENEN UNA ESTRELLA BLANCA CON DOS LÍNEAS HORIZONTALES BLANCAS EN COMÚN:
   <I ID=start></I> (bisnieto de DIV.container)(icono de estrella):
    - Aplicar color **blanco** a la estrella y un tamaño de 31px;

   <HR></HR>(nieto de DIV.CONTAINER)(lineas que van a los lados de la estrella):
    - Aplicar un color **blanco**, una altura de 5px y sin estilos de borde;

   <HR.start-1, DIV .start-1></HR, DIV) (nietos de DIV.container)(Div.start-1 padre de I id=start):
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block) y un ancho de 7% para adecuar el tamaño requerido;

   <DIV id=start-1-icon></DIV>(igual a DIV .start-1, padre de I id=start):
    - Aplicar un ancho de 2.5% para que la estrella este mas junta a las líneas que estan a su lado;

- ESTILOS PARA LAS SECCIONES 1(START BOOTSTRAP) y 3(ABOUT) QUE CONTIENEN UNA ESTRELLA BLANCA CON DOS LÍNEAS HORIZONTALES BLANCAS EN COMÚN:
   <I ID=star-a></I> (bisnieto de DIV.container)(icono de estrella):
    - Aplicar color **negro** a la estrella y un tamaño de 31px;

   <HR.start-2></HR, DIV) (nieto de DIV.container):
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block), un ancho de 7% para adecuar el tamaño requerido y un color **negro**;

- ESTILOS A SECTION 1 (START BOOTSTRAP):
   <H1></H1>(nieto de DIV.container):
    - Aplicar tipo de letra _Montserrat_ con color blanco, con tamaño de letra 80px, con grosor 700 y en mayuscula;    
    - Aplicar un margen inferior de 5px;

   <H3 ID=bootstrap-text"></H3>(nieto de DIV.container):
    - Aplicar tamaño de letra 1.75 em, con grosor 300 y color blanco;
    - Aplicar magen inferior cero;

  <SECTION .start-bootstrap></SECTION>:
    - Aplicar color de fondo  #18bc9c(turquesa);

- ESTILOS A SECTION 2 (PORTFOLIO):
   <H2></h2>(hijos de DIV .container de las sectiones 2,3 y 4):
    - Aplicar tipo de letra _Montserrat_, con tamaño de letra 50px, con grosor 700 y en mayuscula;  

   <DIV .gallery></DIV>(hijo de DIV. container)(galería de imágenes):
    - Aplicar margen izquierdo y derecho de 155px;

   <DIV .images-portfolio></DIV>(nietos de DIV. container, hijo de DIV .gallery)(galería de imágenes):
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block), un ancho de 30% para dividir columnas de tres;
    - aplicar un margen de 13.5px para el espacion entre las imagenes;

  <IMG .images-gallery>(hijo de DIV .images-portfolio ) (imagenes de la galeria):
    - Aplicar un ancho maximo de ancho de 100% para que cada imagen se ajuste a  su contenido en un 100%;

- ESTILOS A SECTION 3 (ABOUT):
   <SECTION id=about></SECTION>:
    - Aplicar color de fondo  #18bc9c(turquesa);

   <H2 id=title-about></H2>:
    - Aplicar color de letra blanco;

   <DIV .information></DIV>(hijo de DIV .container):
    - Aplicar un margen y relleno izquierdo y derecho de 155px y 102px respectivamente;

   <DIV .information-column></DIV>(nieto de DIV .container, hijo de DIV .information):
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block), un ancho de 35% para dividir columnas en dos;

   <P .text-about></P>(hijos de DIV .information-column)(textos de section _About_ en dos columnas):
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block);
    - Aplicar un tamaño de letra de 20px, con un grosor de 400,con color blanco y alineación del texto hacia la izquierda;

   <A .download></A> (nieto de DIV .information-column ):
    - Aplicar un borde radio de lineas solidas de 2px de color blanco;
    - Aplicar un tamaño de letra de 20px, con un grosor de 400;
    - Aplicar un relleno de 7px;

- ESTILOS A SECTION 4 (CONTACT):
   <DIV .form></DIV>( hijo de DIV .container):
    - Aplicar un margen izquierdo y derecho de 155px;

   <FORM .form-1></FORM>(hijo de DIV .form):
    - Aplicar un margen izquierdo y derecho de 230px;

   <DIV .data></DIV>(hijos de FORM .form-1):
    - Aplicar un borde inferior de linea sólida de 1px de color gris;
    - Aplicar un relleno superior e inferior de 33px;

   <INPUT .input-text>(hijos de DIV .data):
    - Anular estilos de borde y relleno izquierdo y derecho;
    - Aplicar un tamaño de letra 1.5 em y un ancho de 100% para que ocupen el ancho necesario;

   <BUTTON></BUTTON> (contiene al botón "send"):
    - Aplicar un display block para asignarle position relative con valor left de cero;
    - Aplicar un tamaño de letra 1.3 em, con grosor de 400 y color blanco;
    - Aplicar color de fondo turquesa, un borde radio de 7px y un relleno de 12px;

- ESTILOS AL FOOTER:
   <FOOTER></FOOTER>:
    - Aplicar color de fondo negro (#2c3e50);

   <DIV .footer-above></DIV> (hijo de footer):
    - Limpiar con clear:both para que **float**(aplicado a su hijo) no afecte a los elementos externos;

   <DIV .column-footer>  </DIV> (nietos de DIV .footer-above):
    - Aplicar color de letra blanco, un margen inferior de 30px;
    - Aplicar **float** con un ancho de 30% para dividirlo en 3 columnas;

   <H3></H3> (hijos de DIV .column-footer):
    - Aplicar tipo de letra _Montserrat_, con tamaño de letra 1.6rem, con grosor 700 y en mayuscula;
    - Aplicar un margin inferior y superior de 30px y 25px respectivamente;

   <P .text-footer></P> (hijos del segundo DIV .column-footer):
    - Aplicar un tamaño de letra 20px y un margen inferior de 80px;

   <DIV .network-icon></DIV>(nietos del segundo DIV .column-footer)(iconos de red social):
    - Aplicar un borde radio de 100% con lineas solidas de 2px color blanco;
    - Aplicar display en linea pero manteniendo la propiedad de bloque (inline-block);
    - Aplicar un margen de 4px, un relleno superior e inferior de 10px izquierda y derecha de 7px;

   <DIV id=facebook, DIV id=google></DIV>(nietos del segundo DIV .column-footer)(iconos de red social):
    - Aplicar un relleno inferior y superior de 10px, un relleno izquierdo y derecho de 10px para facebook y 4.1 para google;

   <I .fa></I> (nietos de DIV .network-icon)(iconos de red social):
    - Aplicar tamaño de letra 20px;

   <A id=footer-link></A> (nieto del tercer DIV .column-footer):
    - Aplicar color de letra turquesa y aplicar un a pseudoclase hover con decoración urderline;

   <H4></H4> (nieto de DIV .footer-below):
    - Aplicar un tamaño de letra 15px, con un grosor ligther y color blanco;
    - Posicionar en forma "relative" hacia la derecha (230px);
    - Aplicar un margen inferior de 7px y un ancho de 60%;

## Estructura

![Freelancer estructure](https://github.com/MariacristinaOrtiz/freelancer/blob/master/assets/docs/estructure-freelancer.png)

## Imagen usado para el replicado

![Freelancer Website](https://github.com/MariacristinaOrtiz/freelancer/blob/master/assets/docs/fullpage.png)
