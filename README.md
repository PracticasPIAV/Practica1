Práctica 1 - PIAV
Autores: Alejandro Bolaños García y David García Díaz

Introducción
Esta práctica tiene como objetivo el desarrollo de un programa interactivo en Python que permita manipular imágenes y crear figuras en un lienzo digital mediante el uso del ratón. Utilizando la biblioteca OpenCV, se implementan funciones para cargar y visualizar imágenes, obtener valores de color en tiempo real, y dibujar diversas figuras geométricas.

Desarrollo
Ejercicio 1a: Visualización de Valores RGB
El primer ejercicio se centra en la interacción con una imagen, de manera que el usuario pueda ver el valor RGB de cualquier píxel al pasar el cursor sobre él. Esto se logró mediante la configuración de eventos de ratón en OpenCV, que permiten capturar la posición del cursor y recuperar los valores de color en esa posición.

Cada vez que el cursor se mueve sobre la imagen, el programa obtiene los valores de los canales de color y los muestra en pantalla en tiempo real, permitiendo al usuario explorar los colores de cualquier punto de la imagen de manera intuitiva.

Ejercicio 1b: Dibujo de Figuras Geométricas
En este ejercicio se habilita la funcionalidad para dibujar figuras geométricas en un lienzo interactivo. Para esto, se emplea un sistema de detección de eventos que captura las acciones del ratón: al hacer clic izquierdo y arrastrar, el usuario puede definir el tamaño y la posición de las figuras. Además, se añadieron controles visuales en forma de barras deslizantes (trackbars), que permiten ajustar características como el color y el grosor de las figuras antes de dibujarlas.

Cada figura cuenta con un modo de dibujo específico, que se puede activar mediante teclas de acceso rápido como se indica en la ventana de leyenda, facilitando la selección y alternancia entre diferentes tipos de formas sin interrumpir la experiencia de dibujo. La implementación de esta funcionalidad permite crear un entorno de dibujo intuitivo, donde el usuario puede ver el efecto de cada configuración en tiempo real.

Mejoras Implementadas
Para ampliar la funcionalidad del programa y ofrecer una experiencia de usuario más rica, se añadieron varias mejoras:

Opción de Relleno para las Figuras: Se incluyó una opción para alternar entre el relleno y el contorno de las figuras. Esta opción es configurable mediante una barra de control y permite al usuario seleccionar si quiere que las figuras sean sólidas o huecas, ofreciendo mayor flexibilidad en el diseño de cada forma.
Nuevas Figuras Geométricas: Además de las figuras básicas, se añadieron polilíneas, polígonos y elipses, lo que incrementa la variedad de formas disponibles en el programa. En el caso de las polilíneas y polígonos, el usuario selecciona varios puntos con el clic izquierdo y con el clic derecho forma la figura final. Esta funcionalidad fue desarrollada utilizando eventos adicionales del ratón, en este caso el evento de clic derecho, para que el usuario pueda dibujar este tipo de figuras con facilidad.
Grabación en Video del Proceso de Dibujo: Se implementó la opción de grabar el proceso de creación en un video. A medida que el usuario dibuja cada figura en el lienzo, el programa captura el estado actual y lo guarda en un archivo de video. Esto permite revisar el proceso completo de dibujo posteriormente y facilita el análisis o la documentación del trabajo realizado.
Aportaciones propias: Como aportaciones propias se añadió la opción de capturar el estado actual del lienzo y guardarlo como imagen mediante una tecla de acceso rápido. Además de poder limpiar el lienzo con otra tecla. Todo esto se indica en la leyenda para que el usuario sepa como utilizar la interfaz.
Conclusión
Esta práctica nos permitió introducirnos a la asignatura de una manera muy interesante, adentrandonos en el mundo de los eventos del ratón y las funciones de callback de OpenCV. Nos sorprendió la versatilidad de las herramientas de OpenCV para estos fines, especialmente en lo relativo a la personalización de los atributos de las figuras.

Al principio, habíamos implementado el segundo ejercicio en una única ventana, donde tanto el lienzo como los trackbars compartían el espacio. Sin embargo, esto resultó poco práctico, ya que el área de dibujo se quedaba reducida y no permitía una visualización adecuada de las figuras. Después de probar esta configuración, decidimos separar el lienzo y los trackbars en dos ventanas independientes, lo que mejoró significativamente la usabilidad del programa. Además, agregamos una leyenda de teclas de acceso rápido, lo cual facilita el uso y permite al usuario alternar rápidamente entre las diferentes opciones de dibujo.

En general, esta práctica fue un aprendizaje muy enriquecedor. Nos permitió enfrentar y resolver problemas de diseño de interfaz y optimización del espacio de trabajo, y nos dejó una mayor comprensión sobre la gestión de eventos y el procesamiento de imágenes. Además, la opción de grabación en video le da un valor añadido al programa, haciéndolo útil para documentar el proceso de dibujo. Consideramos que estos conocimientos serán útiles en futuros proyectos que requieran el desarrollo de herramientas gráficas interactivas y de visualización.
