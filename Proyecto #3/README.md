#Bit

la plataforma nand2tetris nos facilita el codigo del DFF el cual almacenara el valor de el bit, dicho DFF mandara una señal cada sierto tiempo lo que mandara la salida a un multiplexor normal y eso definira la entrada al DFF, ese va a ser el valor que almacene el bit.

#Registrer

El registrer es almacenar 16 bits, por lo que con las entradas llamamos la funcion realizada anteriormente 16 veces.

#RAM8

Como su nombre lo dice, es una memoria que tendrá 8 "slots" para guardar los datos. Para determinar donde se guardan los datos se tiene una entrada llamada "address" que giardará los in de 'in[16]', además del Dmux Que determinará el lugar, El chip Mux se encarga de realizar la impresión del espacio donde está guardado el dato.

#RAM64

Así como la RAM8, se utilizarán 8 veces el chip RAM8 para lograr 64 entradas en la memoria, gracias al vector address con 6 espacios, se puede determinar en que unidad de RAM8 se guardará el dato y en que espacio de esta unidad.

#RAM512

De aquí en adelante todas estas RAM siguen un proceso "recursivo" utilizando los chips anteriores para hacer sus procesos, en esta RAM512 tenemos 8 chips RAM64 para conseguir los 512 que necesitamos, siendo que aquí la entrada address es de 9, en los tres primeros escogerá en que unidad de RAM64 guardará el dato, y los restantes se guardarán donde se les ha asignado.

#RAM4K

Como en las anteriores, en este caso se utilizará el chip RAM512 en 8 repeticiones para conseguir los 4000 espacios necesarios para la operación, el address tiene 12 entradas donde, evidentemente, en las 3 primeras se decide en que RAM512 se hará el guardado y los demás pararan a guardarse.

#RAM16k

Para esta, se repite el mismo proceso solo que está vez utilizaremos nuestro chip anterior, RAM4K, para utilizarlo 8 veces y que nos dé 16000 espacios, donde el address tiene 14 entradas, las 3 primeras son para determinar enque unidad de RAM4k se guardarán las entradas restantes.

#PC

Para realizar el pc primero definimos que va a realizar dicho PC, en este caso va a realizar un incremento, y va a tener tres funciones, que son load, para cargar lo que ya tiene, set para volver el bit a cero y inc que va a ser la operacion de incrementar, para desarrollar el pc lo primero es con la entrada realizar el incremento, luego con tres multiplexores de dieciseis definimos cual de las tres operaciones se van a realizar, con la operacion realizada se guarda en un register.
**¿Por qué el lenguaje de máquina es importante para definir la arquitectura computacional?**

Es esencial porque es la forma en que los bits y bytes se comunican y se entienden dentro del hardware. Piénsalo como el código raíz que la computadora comprende directamente. Sin él, los programas simplemente no podrían hacer que las cosas sucedan dentro de la máquina.
#PREGUNTAS ADICIONALES
**¿Qué diferencia ven entre arquitectura computacional, arquitectura de software y arquitectura del sistema? Justifique su respuesta.**

La arquitectura computacional sería como los cimientos y la estructura básica de la casa, La arquitectura de software sería como la decoración interior y el diseño de cómo interactúan las partes del software.
