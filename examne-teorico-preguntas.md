# EXAMEN TEÓRICO PERIODISMO DE DATOS
### ELENA ROMERO VARGAS
### GRUPO 63

## PREGUNTAS

### Explica la diferencia entre filas y columnas
Tanto las filas como las columnas son elementos que conforman las tablas de datos. Las filas son hileras horizontales que recogen las "líneas" del archivo. Las columnas son las hileras verticales en las que ponemos el tipo de dato con el que estamos trabajando. 

### Explica los pasos para clonar en tu ordenador un repositorio de Github
En primer lugar, tenemos que entrar en la terminal y poner el comando `git clone` y la url del repositorio que queramos clonar. 
Este paso creará una carpeta de nombre similar al repositorio en nuestro ordenador. 
A continuación, con el comando `cd` nos ubicamos en esa carpeta, es decir, dentro del repositorio. Si queremos cambiar algo, lo hacemos con `nano`. 
Si lo que queremos es clonar un repositorio ajeno e interaccionar con él, debemos hacer un fork en Githab para poder crear una copia en nuestra cuenta. 

### Explica los pasos para crear un repositorio en GitHub y conectarlo con un repositorio local
En primer lugar, debemos crear un repositorio en GitHub (tan sencillo como localizar en la cuenta la pestaña de *repositorie* y clicar en *new*). 
Una vez tengamos nuestro repositorio creado, copiamos el link y vamos a la terminal. Allí hacemos `git clone` y pegamos la url del repositorio que hemos copiado antes. Esto creará una carpeta de nombre similar en nuestro ordenador. Para saber dónde nos encontramos, hacemos `pwd` y `cd` hasta llegar a esta carpeta. 
El siguiente paso es incluir lo que queramos en ella: o bien copiamos y pegamos manualmente, o bien abrimos un `nano` para modificar o crear un documento nuevo. 
Los siguientes pasos son: 
- Guardar el nano (Ctrl+X, Y)
- `git add .`
- `git commit .`
- `git push` (en mi caso, en este paso me piden el username y el token, aunque no es común en todos los ordenadores)

### Realiza algún cambio en tu repositorio local y actualízalo también en Github. Explica los pasos. 
Pasos para actualizar un repositorio local: 
1. `git add nombre-archivo-cambiado y/o nombre carpetas o .` (este último si queremos añadir todo)
2. `git commit -m "comentario del cambio` para firmar el cambio
3. `git push main origin` para subirlo a la rama main del repositorio definido como "origin" (para saber cómo hemos definido el repositorio, podemos usar `git remote -v`

### ¿Cómo ves todos los dialectos de la shell disponibles?
Para ver todos los dialectos de shell disponibles se emplea el comando `cat/etc/shells`
Entre estos dialectos están:
- `/bin/bash`
- `/bin/csh`
- `/bin/dash`
- `/bin/ksh`
- `/bin/sh`
- `/bin/tcsh`
- `/bin/zsh`
Para saber qué shell estamos utilizando, el comando empleado es `echo $SHELL`

### Pon varios ejemplos (mínimo, 5) de Google Dorks u "operadores de búsqueda"
- “término de búsqueda”: fuerza una búsqueda de coincidencia exacta
- define: diccionario integrado en Google
- allintitle: devuelve los resultados con todas las palabras especificadas en el título
- - : excluye un término o frase (p.ej → jobs -Apple (las páginas devueltas estarán relacionadas con jobs, pero no con Apple (la empresa))
- [ ]: agrupa varios términos u operadores de búsqueda para controlar cómo se ejecuta la búsqueda
- $: busca precios
- OR: buscar X o Y
- AND: buscar X e Y
- filetype: restringe los resultados a un determinado tipo de archivo
- related: encuentra sitios relacionados a un determinado dominio

### ¿Qué otros comandos o expresiones le pasarías a `lolcat`? Pon ejemplos.
`lolcat` es un comando que convierte todo lo que pasa por él en un "arcoíris". Cualquier comando puede pasar por `lolcat`, pero algunos de ellos son `ls -a |` para listar en colores o `cowsay` para obtener el dibujo de una vaca de colores. 

### Pon ejemplos de uso de los operadores de buscadores y sus resultados
- weather: busca el clima para un lugar específico. Esto se muestra en un snippet de tiempo, pero también devuelve los resultados de otros sitios web sobre el “estado del tiempo”
Ejemplo: weather:san francisco
- stocks: muestra la información bursátil (es decir, el precio, etc.) para una empresa específica.
Ejemplo: stocks:aapl
- map: hace que Google muestre resultados de los mapas para una búsqueda de localización.
Ejemplo: map:silicon valley
- movie: encuentra información sobre una película específica. También encuentra los horarios si la película se muestra actualmente cerca de ti.
Ejemplo: movie:steve jobs
- source: encuentra resultados de noticias de una determinada fuente en Google Noticias.
Ejemplo: apple source:the_verge

### Baja el código fuente de una página web y pásale lolcat. Pega el comando y haz una captura de pantalla y compártela.
ctrl+u para ver el código de una página web 

### ¿Cómo verías el contenido que has descargado? Puedes hacerlo de más de una manera, explica por qué has elegido esa/s opción/es.
En primer lugar, comenzamos por localizar la carpeta en la que hemos descargado el archivo con `cd`. Una vez en ella, hacemos `ls` para listar todo lo que hay dentro. Si el archivo que hemos descargado es oculto, tenemos que hacer `ls-a` para verlo. 

### Contrasta el uso que haces del ordenador con el uso que proponía Doug y explícalo. Puedes ayudarte de una tabla. ¿Qué cosas permanecen y qué ha cambiado?
Doug Engelbert presentó en 1968 en los Xerox Labs de Palo Alto *The mother of all demos*, la primera demsotración pública de un sistema informático fruto de años de investigación sobre las posibilidades que podía ofrecer un ordenador en materia de información y trabajo con datos. 
Con esta demostración, Doug demostró que los ordenadores eran más que "calculadoras gigantes", que permitían trabajar con grandes volúmenes de información y aumentar así las posibilidades humanas. 
En la actualidad, y gracias a avances como este, es posible multiplicar los usos de los ordenadores. Existen muchos más programas y, con la formación correcta, una infinidad de formas de tratar al ordenador. Pero lo más interesante y novedoso es que las actualizaciones de hoy en día permiten que incluso las personas con menos formación en la materia puedan hacer de sus ordenares sus mejores aliados para las tareas del día a día, como pretendía mostrar Doug con su demostración. 

### Qué son las entidades HTML y cómo se representan. Por un ejemplo
Las HTML son caraceteres no comunes que deben presentarse con un código hexadecimal puesto que no son los propios de ASCII (American Standard Codification for Information Exchange). 
Su objetivo es lograr una representación más sencilla de los caracteres que no se incluyen en el alfabeto inglés (por ejemplo, nuestra ñ), sin necesidad de recurrir al código hexadecimal. 
Los strings de las HTML comienzan por un & y finalizan con ;. Estas entidades nos ayudan a conocer mejor todos los lenguajes informáticos que existen, pues nos revela caracteres que en estos lenguajes están reservados. 

###  Dado el significado que tienen las comillas para el comando echo, ¿cómo harías para que devolviera una frase como: La Justicia europea considera "discriminatorio" el sistema de financiación del bono social de las eléctricas (Fuente: [Eldiario.es](https://www.eldiario.es/economia/justicia-europea-considera-discriminatorio-sistema-financiacion-bono-social-electricas_1_8394400.html)?
El comando `echo` se ejecuta para la impresión en pantalla. Lo utilizamos con datos string (cadena de caracteres). 
Si utilizamos entrecomillado simple (‘string’), delimitamos la línea de caracteres. En el caso de usar el doble entrecomillado, conseguiremos expandir los nombres de la variable.

### Pon un ejemplo de uso de "wildcards".
A la hora de listar, copiar, mover y otras operaciones se pueden usar las wildcards o comodines.
Por ejemplo, si como hemos visto en la práctica, tenemos una carpeta en el escritorio llamada data con archivos .csv, .json y .xls, todos juntos, y queremos organizarlo, tenemos que: 
- Situarnos en el directorio data con `cd`
- Crear carpetas con `mkdir`: `mkdir json csv xls`
- Mover archivos con `mv`: `mv archivo.json json/`

*A PARTIR DE AQUÍ ESTÁ COPIADO TAL CUAL*

### ¿Cómo listamos también los archivos y directorios ocultos? Pon un ejemplo.
Para listar los archivos y directorios ocultos se emplea el comando `ls -a`. Si queremos que esta lista ofrezca más detalle, entonces usaremos `ls -la`. 
Los archivos y directorios ocultos contienen configuraciones o datos a los que acceden los programas de ese usuario. No están destinados a ser editados por el usuario, solo por la aplicación Por eso están ocultos de la vista normal del usuario. 
- `ls`: listamos archivos y directorios
- `ls -a`: listamos archivos y directorios ocultos.
- `ls -la`: listamos archivos y directorios ocultos con detalle.

### ¿Qué función tiene la almohadilla en Markdown y en un programa de la shell? Razona tu respuesta.
En los archivos de configuración de la `shell`, sirve para introducir comentarios. La almohadilla `#` que aparece al principio de línea significa que esa línea está comentada y que no va a ser interpretada por la shell. Pueden quedar varias líneas comentadas y son útiles para documentar los pasos que vas dando a lo largo de tu shell script (o guión de shell).
En Markdown equivale al elemento `h1` de HTML o "encabezamiento de primer nivel". Es decir, que las almohadillas se utilizan para crear encabezados. Estos pueden ser de distintos tamaños si se siguen agregando almohadillas, de modo que, a mayor número de almohadillas, menor tamaño del encabezamiento (por ejemplo, dos almohadillas, ##,  darían lugar a un encabezamiento de segundo nivel) Asimismo, para usarlo, se debe añadir uno por cada nivel.

*faltan algunas, mirar en PDF*

### ¿Cuál fue el comienzo del CAR (Computer Assisted Reporting)?
El CAR es el periodismo asistido por ordenador (en español Informes Asistidos por Computadora) y describe el uso de ordenadores para recopilar y analizar los datos necesarios para redactar noticias. Está estrechamente ligado al periodismo de "precisión" o analítico, que se refiere al uso de técnicas de las ciencias sociales y otras disciplinas por parte de los periodistas.
Hay investigadores que sostienen que la "era de la información asistida por ordenador" comenzó en 1952, cuando la cadena de televisión CBS utilizó un ordenador UNIVAC I (la primera computadora comercial fabricada en Estados Unidos) para analizar los resultados de las elecciones presidenciales de EE.UU. 
Uno de los primeros ejemplos se produjo en 1967, tras los disturbios en Detroit, cuando Philip Meyer, del Detroit Free Press, utilizó un ordenador central para demostrar que las personas que habían asistido a la universidad tenían la misma probabilidad de haberse amotinado que las que habían abandonado la escuela secundaria. 
Años más tarde, en su libro *Precision Journalism* (1973), Philip Meyer sostiene que un periodista debe utilizar bases de datos y encuestas, ambas asistidas por ordenador. En la edición de 2002, va más allá y afirma que "un periodista tiene que ser un gestor de bases de datos".

### ¿Qué lenguajes informáticos conoces? Razona la respuesta.
- Lenguajes de programación: Python, R, que hemos aprendido a trabajar desde JupyterHub.
- Lenguajes de marca: HTML
- Protocolos de comunicaciones: http (protocolo de transferencia de hipertexto)
- Otros: Markdown (es un lenguaje de marcado ligero, que nace como herramienta de conversión de texto plano a HTML)

### ¿Cuál es la diferencia entre Internet y la Web? Razona la respuesta.
La web es uno de los servicios de Internet. Internet es la red de redes, es una red global y física por la que circula la información; un conjunto de redes interconectadas a escala mundial. Internet engloba a todas las redes. Los ordenadores integrados en las redes que forman la red Internet son capaces de comunicarse entre sí porque todos ellos utilizan el mismo idioma: los protocolos de comunicación TCP/IP.
Las redes que forman parte de Internet son de muy diversa índole, propósito y tamaño. Hay redes públicas y privadas; locales, regionales e internacionales; instituciones, educativas, universitarias, dedicadas a la investigación, al entretenimiento, etc. La Web solo es una de estas redes; un sistema de hipertexto que funciona gracias a Internet. La World Wide Web (red informática mundial) es un servicio que fue desarrollado en el CERN entre 1989-99 gracias al inglés Tim Barners-Lee. Se fundamenta en dos conceptos: la navegación por medio de hipertexto y la posibilidad de acceder a documentos multimedia.
Existen, por tanto, muchos otros servicios y protocolos en internet, aparte de la Web: el envío de correo electrónico, la transmisión de archivos,  las conversaciones en línea, la mensajería instantánea, la transmisión de contenido y comunicación multimedia, los juegos en línea…

### ¿Qué fue determinante para el nacimiento del periodismo de datos moderno?
El periodismo de datos tal y como lo conocemos hoy, el periodismo de datos moderno nacido en los años 2006-2008, surge en un momento en el que coincidieron una serie de circunstancias en la evolución histórica de Internet que posibilitaron su forma: 
- Abundancia de código abierto (también llamado software abierto, “software que podemos usar, escribir, modificar y redistribuir libremente”, que los desarrolladores de software o programadores de código decidan publicar y compartir su trabajo sin reservarse sus derechos de autor exclusivos para sí, sino que compartan su trabajo y que este forme parte del dominio público), algo que promueve ampliar la participación, la colaboración y el aprendizaje. 
- HTML5. La quinta versión de nuestro lenguaje básico de la World Wide Web (=el ecosistema de páginas de Internet). Fue lanzada inicialmente en 2014. Es el estándar con el que están programadas todas las webs hoy día, y aunque algunas puedan tener elementos o fragmentos programados en otros lenguajes, siempre tienen que ser "encajados" en el total con este lenguaje. Incorpora respecto al HTML4 algunas novedades interesantes. Una de las notables es darle cobertura a la reproducción de contenido multimedia, de forma que ya no tengas que ir a recursos de terceros (plug-ins) como el obsoleto Flash Player. También incluye programación de aplicaciones, geolocalización… 
- OpenData. filosofía y práctica que persigue que determinados tipos de datos estén disponibles de forma libre para todo el mundo, sin restricciones de derechos de autor, de patentes o de otros mecanismos de control; tiene mucho que ver con el movimiento de código abierto antes mencionado. Se reclama transparencia a instituciones públicas, privadas, investigaciones científicas…

###  ¿Qué saberes están implicados en periodismo de datos? Razona la respuesta. 
El periodismo de datos tal y como lo conocemos hoy, el periodismo de datos moderno nacido en los años 2006-2008, surge en un momento en el que coincidieron una serie de circunstancias en la evolución histórica de Internet que posibilitaron su forma: abundancia de código abierto, HTML5 y OpenData. De ahí surgen los pilares sobre los que hoy se fundamenta y en los que se basa como disciplina:
- Investigación (porque hablar de labor periodística es hablar de investigación)
- Datos (pero no cualquier tipo de datos, sino registros electrónicos que deben tratarse con ordenador)
- Visualización de los datos: a través de la web, infografías, análisis estadísticos y un amplio abanico de visualizaciones. 

### ¿Cuál es la materia del periodismo de datos? Razona la respuesta
Como su propio nombre indica, la materia del periodismo de datos son, efectivamente, los datos. Sin embargo, hay un matiz clave en la naturaleza de esta disciplina: cuando hablamos de datos, no nos referimos solo a datos estructurados o conjuntos de datos, sino que se trata de registros electrónicos (y en esta categoría caben datos estructurados y datos que no lo están, texto, música, imágenes, vídeos, e incluso los patrones de comportamiento del usuario en las aplicaciones y dispositivos electrónicos). Por otra parte, el hecho de llamarlo "periodismo guiado por datos" o *data driven journalism* no debe menospreciar que lo importante es el periodismo. Es decir, hay que saber trabajar con datos como una parte más del trabajo periodístico.

### ¿Qué tipo de interfaces de datos hay?
Existen tres tipos de interfaces: 
- CLI: interfaz de línea de comandos
- GUI: interfaz gráfica de usuarios
- Las de los móviles, que son capacitivas

### ¿Qué tipos de datos hay?
1. Numéricos: Corresponden a un identificador, que en este caso está compuesto por números.
- interger: números enteros, sin decimales. 
- decimal: números con decimales pero pocos decimales y siempre el mismo número de decimales
- float or double:números con muchos decimales de longitud variable
- date or datatime
- period
2. Strings: Cadenas de caracteres
3. Booleanos: Representan dos valores de una lógica binaria: “verdadero o falso”, “true or false”, “sí o no”, “0 o 1”... El nombre se debe a George Boole, "desarrolló un sistema de reglas que le permitían expresar, manipular y simplificar problemas lógicos y filosóficos cuyos argumentos admiten dos estados (verdadero o falso) por procedimientos matemáticos."
