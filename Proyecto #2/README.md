# HALFADDER
Para el desarrollo de este componete observamos su tabla de verdad:
![Imagen de WhatsApp 2024-02-29 a las 16 37 53_4c6f5b94](https://github.com/Fitman22/ArchiTech/assets/70348839/e7d22c49-159d-4123-a2c8-78b8bca3caea)

# FULLADDER
Para la realizacion de este componente lo que se hace es realizar una media suma y el resultado obtenido de esa media suma se le realiza otra media suma, esas dos medias sumas nos generaran dos carrys de salida respectivamente, con los cuales realizaremos un or para definir la salida del carry final.
# ADD16
La funcion de este componente es realizar 16 sumas para lo cual para la primera suma se realiza una media suma, dicha suma nos va a generar un carry, de ahi en adelante con ese carry se realizaran las siguientes 15 sumas completas.
# INC16
Para el desarrollo de esta funcion simplemente se realizara la funcion Add16 pasandole la segunda entrada como un vector de unos, por lo que le realizara un incremento de uno a cada uno de los elementos.
# ALU 
Para el desarrollo de la alu necesitamos tener en cuneta los selectores, lo primero que hacemos es analizar los primeros selectores y utilizar un multiplexor para definir si deja la entrada x y la entrada y o si las transforma en un vector de ceros, seguido a esto tendremos un nuevo valor de y y un nuevo valor de x los cuales vamos a negar o no segun el selector para ello, pasamos a un multiplexor el valor de x y x negado y en otro multiplexor el valor de y y y negado, con esto tendremos dos nuevas salidas de x y y, realizamos la funcion add16 y la funcion and16, y las pasamos a otro multiplexor de 16 el cual nos dira si guarda el valor de la add16 o de la and 16, esta salida se negara y se pasara a otro multiplexor el cual elegira si se deja dicha funcion o si se debe negar la funcion, por ultimo se tiene que analizar la salida ya que si es igual a 0 zr debe retornar el valor de 1 y si la salida es menor que 0 la salida ng debe retornar 1.
# PREGUNTAS ADICIONALES
#¿Cuál es el objetivo de cada uno de esos proyectos con sus palabras y describa que debe hacer para desarrollarlo?

El proyecto 02 se enfoca en construir todos los chips necesarios para completar la ALU. Esto implica diseñar y desarrollar los chips de acuerdo con la funcionalidad y la conectividad requeridas para la ALU. Después del diseño, se procede a implementar los chips y se llevan a cabo pruebas exhaustivas para asegurar que la ALU funcione correctamente según los requisitos específicos del proyecto.

En cuanto al proyecto 03, su objetivo principal radica en construir los chips utilizando como base el diseño del DFF (Flip-Flop D) y los chips desarrollados previamente. Este proceso implica crear los nuevos chips tomando como referencia el diseño del DFF y utilizando los chips existentes como componentes esenciales en su construcción.

##Explique las principales diferencias entre la lógica aritmética y la lógica secuencial.

La lógica aritmética se encarga de realizar cálculos numéricos y operaciones como sumas, restas, multiplicaciones y divisiones, además de tomar decisiones lógicas. En contraste, la lógica secuencial se dedica a almacenar y procesar información en una secuencia que depende de eventos previos.

Los circuitos de lógica aritmética se diseñan para ejecutar operaciones básicas utilizando principalmente compuertas lógicas, multiplexores y otros componentes para realizar cálculos y manipular datos. Por otro lado, los circuitos de lógica secuencial se basan en la memoria y emplean elementos como flip-flops, contadores, registros y máquinas de estado para controlar y mantener estados internos a lo largo del tiempo.

En términos de salida, la lógica aritmética combina varias entradas para producir una salida, mientras que la lógica secuencial puede tener múltiples salidas que dependen del estado actual del circuito.
