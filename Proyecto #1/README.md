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

Se implementa la compuerta lógica AND de 16 bits, denominada `And16`. Esta compuerta toma dos entradas de 16 bits (`a[16]` y `b[16]`) y produce una salida de 16 bits (`out[16]`), donde cada bit de salida es el resultado de la operación AND lógica correspondiente entre los bits de entrada. Para lograr esto, el código utiliza 16 compuertas AND individuales (`And`) para realizar la operación AND entre cada par correspondiente de bits de las entradas `a` y `b`. Cada compuerta AND toma un par de bits de las entradas `a` y `b`, y produce el resultado correspondiente, que se asigna al bit correspondiente de la salida `out`.

# OR16

Se implementa la compuerta lógica OR de 16 bits, denominada `Or16`. Esta compuerta toma dos entradas de 16 bits (`a[16]` y `b[16]`) y produce una salida de 16 bits (`out[16]`), donde cada bit de salida es el resultado de la operación OR lógica correspondiente entre los bits de entrada. Para lograr esto, el código utiliza 16 compuertas OR individuales (`Or`) para realizar la operación OR entre cada par correspondiente de bits de las entradas `a` y `b`. Cada compuerta OR toma un par de bits de las entradas `a` y `b`, y produce el resultado correspondiente, que se asigna al bit correspondiente de la salida `out`.

# MUX16

# OR8WAY

Se implementa la compuerta lógica OR de 8 vías, llamada `Or8Way`. Esta compuerta tiene 8 entradas (`in[8]`) y produce una única salida (`out`). La salida es verdadera (1) si al menos una de las entradas es verdadera (1). Para lograr esto, el código utiliza varias compuertas lógicas OR para realizar la operación OR entre diferentes grupos de entradas. Se agrupan las entradas en pares, y luego se realizan operaciones OR entre los pares de entradas. Posteriormente, se realizan operaciones OR entre los resultados intermedios hasta obtener la salida final.

# MUX4WAY16

El chip `Mux4Way16` es un multiplexor de 4 vías de 16 bits. Esto significa que toma cuatro conjuntos de datos de entrada, cada uno de 16 bits (`a`, `b`, `c` y `d`), y selecciona uno de estos conjuntos de datos de salida basado en dos señales de selección (`sel[0]` y `sel[1]`). El propósito principal de este chip es seleccionar entre cuatro entradas diferentes (`a`, `b`, `c` y `d`) para dirigir a la salida (`out`), dependiendo de los valores de las señales de selección (`sel[0]` y `sel[1]`). 

Internamente, el chip utiliza tres chips Mux16 (multiplexores de 16 bits) para realizar esta operación. Dos de estos Mux16 se utilizan para seleccionar entre `a` y `b`, y entre `c` y `d`, respectivamente, basándose en el valor de la primera señal de selección (`sel[0]`). Los resultados de estas dos operaciones de multiplexación se almacenan temporalmente en `tout1` y `tout2`. Luego, otro chip Mux16 se utiliza para seleccionar entre `tout1` y `tout2`, dependiendo del valor de la segunda señal de selección (`sel[1]`). El resultado final de esta operación se dirige a la salida `out`.

# MUX8WAY16

El chip `Mux8Way16` es un multiplexor de 8 vías de 16 bits. Esto significa que toma ocho conjuntos de datos de entrada, cada uno de 16 bits (`a`, `b`, `c`, `d`, `e`, `f`, `g` y `h`), y selecciona uno de estos conjuntos de datos de salida basado en tres señales de selección (`sel[0]`, `sel[1]` y `sel[2]`). El propósito principal de este chip es seleccionar entre ocho entradas diferentes (`a`, `b`, `c`, `d`, `e`, `f`, `g` y `h`) para dirigir a la salida (`out`), dependiendo de los valores de las señales de selección (`sel[0]`, `sel[1]` y `sel[2]`).

Internamente, el chip utiliza dos chips `Mux4Way16` (multiplexores de 4 vías de 16 bits) para realizar esta operación. El primer `Mux4Way16` selecciona entre los conjuntos de datos `a`, `b`, `c` y `d` basándose en los dos bits más bajos de la señal de selección (`sel[0]` y `sel[1]`), y almacena el resultado temporalmente en `tout1`. El segundo `Mux4Way16` selecciona entre los conjuntos de datos `e`, `f`, `g` y `h` también basándose en los dos bits más bajos de la señal de selección (`sel[0]` y `sel[1]`), y almacena el resultado en `tout2`. Luego, un chip `Mux16` se utiliza para seleccionar entre `tout1` y `tout2`, basándose en el tercer bit de la señal de selección (`sel[2]`). El resultado final de esta operación se dirige a la salida `out`.

# DMUX4WAY

El chip `DMux4Way` es un demultiplexor de 4 vías. Toma una entrada `in` y la dirige a una de las cuatro salidas (`a`, `b`, `c` y `d`), basándose en dos señales de selección (`sel[0]` y `sel[1]`). Internamente, el chip utiliza dos instancias del chip `DMux` (demultiplexor) para realizar esta operación. El primer `DMux` divide la entrada `in` en dos salidas, `tout1` y `tout2`, basándose en el valor de la señal de selección `sel[1]`. Luego, cada una de estas salidas se divide nuevamente utilizando otro `DMux` basándose en el valor de la señal de selección `sel[0]`. El resultado de estos `DMux` es dirigido a las salidas `a`, `b`, `c` y `d`.

# DMUX8WAY

El chip `DMux8Way` es un demultiplexor de 8 vías. Toma una sola entrada `in` y la dirige a una de las ocho salidas (`a`, `b`, `c`, `d`, `e`, `f`, `g` y `h`) basándose en tres señales de selección (`sel[0]`, `sel[1]` y `sel[2]`). Para lograr esto, el chip utiliza una combinación de puertas lógicas y demultiplexores de menor tamaño. En primer lugar, se niega la señal de selección `sel[0]` utilizando un chip `Not`, y se realiza una operación AND entre la entrada `in` y la señal negada `tsel1`, lo que resulta en la salida `Inout`. Esta señal `Inout` se utiliza para dirigir la entrada a uno de los dos demultiplexores 4-vías (`DMux4Way`), dependiendo de los valores de `sel[1]` y `sel[2]`.

Por otro lado, la entrada `in` se combina con la señal de selección `sel[0]` utilizando una operación AND para producir la señal `Inout1`, que se utiliza para dirigir la entrada a otro demultiplexor 4-vías en función de los valores de `sel[1]` y `sel[2]`.


# PREGUNTAS ADICIONALES
**1. ¿Qué consideraciones importantes debe tener en cuenta para trabajar con Nand2Tetris?**

**Nand2Tetris** es un software que nos ayuda a entender el funcionamiento de las compuertas lógicas. Para poder utilizar este programa de manera satisfactoria, es necesario saber cómo funcionan las compuertas lógicas, ya que se deben crear diversas compuertas como Not, Or, And, entre otras, usando únicamente una compuerta Nand primitiva.

**Se debe conocer:**

- Qué bits le deben llegar a cada compuerta para obtener una salida determinada.
- Con cuál operador binario funciona cada compuerta, si esta trabaja con uno solo o usa varios operadores.
- Si el resultado de estas operaciones se debe negar, como es el caso de la Nand.

Una vez que se entiende este tema, es muy sencillo usar el software de Nand2Tetris. Solo se debe recordar tener la última versión de Java, puesto que trabaja en base a este lenguaje de programación.

**2. ¿Qué otras herramientas similares a Nand2Tetris existen?**

Existen diversas herramientas que te ayudan a entender el funcionamiento de un computador, algunas de ellas son:

- **LC-3 Simulator:** Es un computador educativo de 16 bits diseñado para enseñar los fundamentos de arquitectura de computadores.
- **Logisim:** Es un entorno de simulación lógica digital. Se utiliza para crear y probar circuitos utilizados en las computadoras.
- **Proteus y Multisim:** Son softwares de diseño de circuitos de circuitos eléctricos, similares a Logisim.
- **Icarus Verilog:** es un simulador de lenguaje de descripción de hardware (HDL).


