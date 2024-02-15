# PRACTICA #1 - ARQUITECTURA DE COMPUTADORES 

En el mundo de la informática y la ingeniería de computadoras, la lógica booleana es fundamental. Se trata de un conjunto de reglas y operaciones fundamentales que gobiernan el comportamiento de las señales digitales en un sistema informático. Este proyecto se centra en la construcción de una serie de puertas lógicas básicas, como And, Or, Mux, entre otras, utilizando exclusivamente puertas Nand primitivas y las puertas compuestas que se construirán gradualmente sobre ellas. Estas puertas lógicas son los bloques de construcción esenciales para la creación de la Unidad Central de Procesamiento (CPU) y la Memoria de Acceso Aleatorio (RAM) de un computador. El objetivo principal del proyecto es la familiarizaicon con los principios fundamentales de la lógica booleana y proporcionar una comprensión práctica de cómo se construyen los circuitos lógicos básicos que forman la base de la arquitectura de una computadora.
                  
# NOT

![image](https://github.com/Fitman22/ArchiTech/assets/124414206/dcc0a095-bfb8-4ae6-bdf1-3b2a3d48c1d5)
         
La implementacion de la compuerta lógica NOT se realizo utilizando una compuerta NAND. La entrada se conecta a ambas entradas de la compuerta NAND, y la salida de la NAND se convierte en la salida de la compuerta NOT, produciendo así la inversión lógica de la entrada.

# AND

![image](https://github.com/Fitman22/ArchiTech/assets/124414206/f30a1f16-fd6f-495f-b0d8-64c492bcd029)

La implementacion de la compuerta lógica AND se realizo utilizando dos compuertas NAND. La salida de la primera NAND proporciona la negación de las entradas `a` y `b`, y luego la segunda NAND calcula la negación de esa salida, produciendo así el resultado de la operación AND lógica de las entradas `a` y `b`.

# OR

![image](https://github.com/Fitman22/ArchiTech/assets/124414206/a3c2648f-78e4-4a51-ab3b-8ee93362a8aa)

La compuerta lógica OR se realizo utilizando únicamente compuertas NAND. El enfoque del código es utilizar la propiedad de universalidad de las compuertas NAND, lo que significa que pueden utilizarse para implementar cualquier otra compuerta lógica. Internamente, el código utiliza tres compuertas NAND. La primera compuerta NAND calcula la negación lógica de la entrada `a` y la segunda compuerta NAND calcula la negación lógica de la entrada `b`. Luego, la tercera compuerta NAND calcula la negación lógica de las salidas de las dos primeras compuertas NAND, lo que resulta en la operación OR lógica de las entradas `a` y `b`.

# XOR

![image](https://github.com/Fitman22/ArchiTech/assets/124414206/7e1399f3-18fd-48bb-8e44-d44a974c40a2)

Claro, aquí tienes una explicación más detallada del código:

La implementacion de la compuerta lógica XOR (Exclusive OR) se realizo utilizando únicamente compuertas NAND. Primero, se calcula la negación lógica de cada una de las entradas `a` y `b` utilizando dos compuertas NAND. Esto produce las señales negadas `nega` y `negb`. Luego, se utiliza una compuerta NAND para calcular la operación OR lógica entre `a` y `b`, utilizando las señales negadas `nega` y `negb`. Esto produce la señal `orout`. Después, se calcula la negación lógica de la señal `orout` utilizando una compuerta NAND, lo que resulta en la señal negada `negout`. Finalmente, se calcula la operación NAND entre las señales `negout` y `negand` para obtener la salida final de la compuerta XOR.

# MUX

# DMUX

# NOT16

Se implementa una compuerta lógica de inversión de 16 bits llamada `Not16`. Esta compuerta toma una entrada de 16 bits (`in[16]`) y produce una salida de 16 bits (`out[16]`), donde cada bit de salida es la inversión lógica del bit correspondiente de la entrada. Para lograr esto, se utilizan 16 compuertas NOT individuales. Cada una de estas compuertas NOT toma un bit de la entrada de 16 bits y produce la inversión lógica de ese bit, que se asigna al bit correspondiente de la salida.

# AND16

# OR16

# MUX16

# OR8WAY

# MUX4WAY16

# MUX8WAY16

# DMUX4WAY

# DMUX8WAY

# PREGUNTAS PRACTICA

# PREGUNTAS ADICIONALES

1. ¿Que consideraciones importantes debe tener en cuenta para trabajar con Nand2Tetris?


2. ¿Que otras herramientas similares a Nand2Tetris existen? 


