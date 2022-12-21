# RETO ACTIVIDAD 3: Visionando el futuro con las gafas de Manovich: redescubriendo la hibridación
### Asignatura de Cultura digital - UOC

**Autor**: Mariano Mayayo Burillo |  **Fecha**: 18/12/2022

----------

## Introducción: ¿Qué es la Hibridación?

A partir de los años 90 se produce una evolución en los nuevos medios tal como hasta entonces eran conocidos, así como en las técnicas utilizadas para crearlos, modificarlos y acceder a ellos. Los medios comienzan a adquirir nuevas propiedades, y gracias a distintas necesidades de los usuarios se empiezan a fusionar entre sí, dando lugar a nuevos medios híbridos. (Manovich, 2013)

La hibridación implica que los distintos medios que componen el nuevo medio creado guardan cierta relación unos con otros. Sus técnicas y los datos que componen estos medios igualmente se relacionan dando lugar a un elemento con nuevas características, lo que genera una experiencia en el usuario diferente a la que ofrecen los medios originales de manera independiente. (Adell, 2014).

Se debe tener en cuenta que la hibridación de medios no es lo que conocemos habitualmente como multimedia. Un producto multimedia, nos muestra una combinación de diferentes medios que técnicamente no se encuentran relacionados entre sí, aunque el contenido o la información que ofrecen sí pueda estarlo. Por ejemplo una web sobre noticias puede albergar textos, imágenes y vídeos, todos ellos medios que poseen propiedades y técnicas diferentes, pero que pueden guardar relación en cuanto a la información que ofrecen.

Para entender un poco más en detalle de qué estamos hablando cuando nos referimos a hibridación, analizaremos brevemente dos casos en concreto: Unreal Engine, un motor de juegos muy utilizado últimamente para producción audiovisual virtual, y WondaVR, una plataforma inmersiva que nos permite crear reuniones y eventos virtuales multiusuario.

## Caso 1.  Hibridación en producción virtual con Unreal Engine

Los motores de juegos son un tipo de software cultural que nos permiten crear y ejecutar todo tipo de experiencias interactivas y de entretenimiento gracias a la combinación de distintos tipos de medios tanto en 2D como en 3D. Este tipo de entornos de desarrollo, además de permitir la programación de los distintos comportamientos que pueden adoptar los elementos que componen el juego, tienen la capacidad de poder mostrar (renderizar) imágenes de escenas generadas por ordenador en tiempo real y con una gran calidad, tanta que en ocasiones es difícil diferenciar una imagen captada por una cámara fotográfica o de vídeo de una imagen creada en uno de estos motores. 

Los distintos avances tecnológicos como el desarrollo de nuevas tarjetas gráficas cada vez más potentes, el desarrollo del software, concretamente algoritmos de renderización de imágenes avanzados y plugins que permiten la interconexión con distintos dispositivos, y la necesidad cada vez mas creciente en producción audiovisual, de creación e integración de imágenes generadas por ordenador con escenas reales, han convertido a estos motores en una nueva herramienta en este sector.

**Unreal Engine**, probablemente el motor de desarrollo de juegos más potente del mercado, es el principal ejemplo de entorno de producción virtual. No solo se usa para crear videojuegos, sino también para crear escenas virtuales complejas con gran nivel de realismo en las que se puede integrar un actor, o un personaje del mundo real dentro de un escenario virtual. Dicho de otra manera, estamos hablando de Realidad Virtual (RV), lo que por definición nos lleva a un claro ejemplo de hibridación de medios ya que nos muestra una representación de una nueva escena que combina elementos reales con imágenes generadas por ordenador y que sería casi imposible crear de otra manera.

![Captura de pantalla de Unreal Engine](https://drive.google.com/uc?id=15AZTTtChlChFbaqyNKx-EwvU3tXk0r3i)  

>Captura de pantalla de proyecto de VR de Unreal Engine. Fuente: mmayayo3d

![Captura de pantalla de Unreal Engine](https://drive.google.com/uc?id=1HEKsx-vvHrvEgV_9rt64xs15P34VXpU)

Para poder crear composiciones de este tipo se suelen utilizar dos técnicas. La primera es la técnica del **Chroma Key**, que consiste en captar mediante una cámara la imagen de un actor o una escena real sobre un fondo de color (normalmente verde) para poder sustituir este fondo por una imagen de un escenario generado por ordenador. La otra técnica que se suele usar en grandes producciones audiovisuales consiste en situar **pantallas LED** en el fondo de la escena para  poder proyectar el escenario creado en la computadora sobre estas pantallas, de manera que la cámara finalmente capta la imagen del actor sobre este nuevo escenario. Técnicamente son formas diferentes de producción virtual, pero, en esencia funcionan de la misma manera, mediante la combinación de una cámara de vídeo y una cámara virtual que genera la escena 3D.

Esta combinación de elementos ya nos da a entender que el resultado final es un nuevo medio híbrido creado a partir de otros medios previamente existentes, y que gracias a las capacidades que ofrece el entorno **Unreal Engine**, este tipo de escenas pueden ser creadas incluso en tiempo real.

### Técnicas y datos

La creación de escenografía virtual implica el uso de varias técnicas procedentes de distintos medios combinadas con otras nuevas desarrolladas específicamente para crear este nuevo medio. A las técnicas tradicionales audiovisuales como pueden ser la grabación en cámara, el **Chroma Key**, o la composición de imágenes por capas, comunes a diversas aplicaciones gráficas, se le suman en este caso otras nuevas como la captura de movimiento, en este caso utilizada para conocer la posición exacta de la cámara (camera tracking) en el espacio real, con el objetivo de poder situar una cámara virtual en la misma posición dentro del espacio 3D. De esta manera el punto de vista que ofrece la cámara real será el mismo que el que ofrece la cámara virtual. Pero no solo debemos conocer la posición y orientación de la cámara. Otro parámetro fundamental a la hora de realizar escenografía virtual es el ángulo de la lente de la cámara, es decir, su distancia focal. Para que el nuevo medio creado resulte creíble, ambas cámaras (real y virtual) deben estar en la misma posición, orientación y con la misma distancia focal en el escenario real y en el escenario 3D.

Y para conseguir este objetivo existen los dispositivos rastreadores de movimiento que generan datos de posición y orientación de un objeto en un espacio físico, y pueden ser enviados a los motores de render. En el caso de dispositivos específicos de posicionamiento de cámara, además pueden ofrecer datos de distancia focal, punto de enfoque, apertura de diafragma etc... Datos del mundo real que pueden ser tratados mediante software y asignados automáticamente a la cámara virtual. 

> **Nota:** Según el principio de automatización de los nuevos medios (Manovich, 2005), hay acciones en la manipulación de los datos que los componen que pueden ser realizadas de manera automática. De manera que si un operador está realizando un movimiento de cámara de plató, automáticamente estará moviendo también la cámara virtual del espacio 3D de manera sincronizada.

### Composición por capas

La imagen final se genera mediante la composición por capas situando en el frente la imagen de vídeo captada en tiempo real por la cámara de plató a la que se le aplica un **Chroma Key**, y en el fondo la escena 3D creada en el entorno virtual. Gracias a la sincronización de ambas cámaras en posición y distancia focal, es posible conseguir una escena en la que el actor se encuentra perfectamente integrado en el nuevo entorno. Casi podríamos decir que es en este momento donde se está produciendo realmente la hibridación de los medios, es decir, se fusiona la imagen del mundo real con la imagen del mundo virtual y se crea una nueva escena hasta entonces inexistente. (Unreal Engine)

###  Resultado y conclusión sobre Unreal Engine

En **Unreal Engine** nos encontramos con un software de medios que nos permite crear nuevos medios híbridos, en el caso de la producción virtual, una nueva escena que combina dos técnicas, una imagen de vídeo y otra generada por ordenador. Aunque finalmente el medio que vemos gracias a este tipo de producción es un vídeo digital, un tipo de medio ya existente previamente, éste ha sido creado mediante la fusión de diversas capas de vídeo y elementos 3d, es decir, hibridando distintos tipos de medios, lo que le da un significado totalmente nuevo al crear una representación de una escena en un nuevo mundo.

Pero no sólo el vídeo final es un medio híbrido, la propia herramienta de desarrollo también lo es. **Unreal Engine** combina técnicas propias de medios concretos como puede ser el tratamiento de señales de vídeo, específico del video digital, o la manipulación de objetos tridimensionales, específico de este tipo de objetos, con otras comunes a todos ellos como puede ser la visualización de los mismos a través de la cámara virtual, o la programación mediante código sobre objetos de distintos medios.

Además de combinar medios y técnicas, es posible generar una nueva interfaz personalizada para el uso y la manipulación del nuevo entorno virtual creado. Por ejemplo es posible incluir elementos de interfaz que nos permiten controlar la distancia focal de la cámara en el plató y a la vez la de la cámara virtual o controlar de manera sincronizada la intensidad de la iluminación real y la virtual. Esta nueva interfaz se puede crear partiendo de elementos preexistentes como botones, campos de entrada de datos, o deslizadores, entre otros elementos, o puede ser diseñada totalmente nueva, pero en cualquiera de los dos casos, sus funciones serán totalmente nuevas y específicas para modificar los datos de este nuevo medio creado.

## Caso 2. Hibridación en WondaVR

WondaVR es una plataforma que nos permite crear espacios virtuales colaborativos en 2D, 3D y 360º. Se utiliza principalmente para aprendizaje, trabajo en equipo y reuniones online. Un administrador puede crear salas, dentro de un mismo espacio 3D, a las que se pueden conectar los asistentes a la reunión de manera online. (WondaVR)

La comunicación entre los usuarios se realiza a través de una llamada similar a las que podemos realizar en las reuniones de Microsoft Teams, o de Zoom con varios usuarios, con la característica principal de que estas reuniones se desarrollan en un entorno virtual creado en la misma plataforma y mostrando a los usuarios como avatares con los que es posible interactuar en el mismo espacio. Para los asistentes se incluyen además opciones para compartir pantalla, una pizarra digital que dibujar o hacer distintas anotaciones, o la posibilidad de incluir nuevos elementos interactivos dentro del espacio.

![Captura de pantalla de WondaVR](https://drive.google.com/uc?id=1S47o-bTVhDWtF565J51lgK71rcc-oFg0)
>Captura de pantalla de dos usuarios en una misma sesión en WondaVR. Fuente: mmayayo3d

Estas características son un claro ejemplo de hibridación de medios. La plataforma en sí es un entorno de desarrollo que podemos englobar dentro de la categoría del software de los medios, y que permite a un creador (administrador) el diseño de las distintas salas de reunión combinando adecuadamente, en un espacio tridimensional, medios de diferentes tipos como imágenes, textos, vídeos o elementos interactivos. El resultado final será un nuevo medio híbrido, una sala de reuniones virtual en la que los medios originales implicados en su creación, ahora forman parte de un todo.

### Datos vs Interfaz

Cualquier tipo de comunicación tiene varios actores fundamentales, como son emisor, receptor, canal y mensaje. En este caso, el mensaje, se transmite como datos codificados al receptor a través de la red. Estos datos constituyen la esencia de la plataforma WondaVR, y la forma de generarlos y mostrarlos es a través de la interfaz de usuario. En función del tipo de mensaje, que queramos transmitir, se utilizará una parte u otra de la interfaz del usuario. De la misma manera en el momento de la recepción de los datos, éstos se mostrarán haciendo uso de distintas partes de la interfaz. Pero debemos tener en cuenta que datos e interfaz pueden estar relacionados entre sí, pero son elementos totalmente independientes. Podríamos estar transmitiendo exactamente el mismo mensaje, los mismos datos, pero mostrarlos de una manera totalmente distinta. Esta misma idea la podemos apreciar en aplicaciones similares como Skype, Google Meet y otras dedicadas a la comunicación grupal.

En WondaVR tenemos el mismo tipo de datos que en cualquier otra aplicación de comunicación entre diferentes usuarios, audio, vídeo, imágenes o textos, pero se muestran de una manera específica dentro de un entorno 3D. Este escenario puede ser creado por el usuario, o generado automáticamente por la plataforma, y los datos que se transmiten, es decir, los mensajes,  ahora se muestran como elementos de la propia interfaz. Podemos compartir una imagen, un vídeo o un archivo de audio, simplemente colocando el objeto en el espacio 3D de manera que puede ser visualizado por el receptor dentro del mismo espacio. Si además es dispositivo utilizado para el acceso a la plataforma es un dispositivo de realidad virtual como pueden ser unas gafas VR, la experiencia del usuario es totalmente inmersiva y los propios movimientos del usuario son ahora controles de interfaz. (WondaVR)

###  Resultado y conclusión sobre WondaVR

WondaVR es una plataforma de comunicación entre múltiples usuarios desarrollada para mostrar los distintos mensajes sobre una nueva interfaz en un espacio tridimensional. La hibridación en este caso se produce en dos aspectos fundamentalmente; se crea una nueva interfaz de usuario para crear, modificar y acceder a los distintos datos que componen los mensajes transmitidos, y además se crea un nuevo entorno que combina distintas técnicas de diversos medios, es decir, una nueva experiencia, a la que acceden los usuarios, de manera que en una única sala creada por software se pueden encontrar personas que físicamente se encuentran en distintas partes del mundo compartiendo la información de diferentes medios en un único espacio, un nuevo medio híbrido. 


## Referencias

ADELL, F (2014). Remediación, multimedia e hibridación de los medios. Mosaic [en línea], 2014. Disponible en: http://multimedia.uoc.edu/blogs/fem/es/remediacio-multimedia-i-hibridacio-dels-mitjans/

MANOVICH, L. (2005). ¿Qué son los nuevos medios? En: El lenguaje de los nuevos medios de comunicación. Barcelona: Paidós, 2005 (p. 63-109)

MANOVICH, L. (2013). El software toma el mando. Barcelona: Editorial UOC. (Capítulos IV y V)

UNREAL ENGINE. Consultado en diciembre de 2022. [En línea]. Disponible en: https://www.unrealengine.com/es-ES

WONDAVR. Consultado en diciembre de 2022. [En Línea]. Disponible en: https://www.wondavr.com




