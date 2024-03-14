# PROYECTO 4 - ARQUITECTURA DE COMPUTADORES

# ¿Por qué el lenguaje de máquina es importante para definir la arquitectura computacional?

El lenguaje de máquina es crucial para establecer la arquitectura computacional, ya que es el idioma que el hardware de la computadora utiliza para procesar instrucciones y datos. Es importante porque permite a la CPU trabajar eficientemente y estructurar los componentes de hardware de manera adecuada. Además, el lenguaje de máquina es el estándar común utilizado para comunicarse con diferentes tipos y modelos de hardware de computadora.

# MULT.ASM

El programa Mult.asm es un programa en ensamblador diseñado para la arquitectura del computador virtual. Este programa específicamente realiza la multiplicación de dos números enteros positivos sin signo, almacenados en las ubicaciones de memoria `R0` y `R1`, y guardar el resultado en la ubicación de memoria `R2`.

El programa utiliza un método de multiplicación por sumas sucesivas. La idea básica detrás de este algoritmo es repetir la suma del multiplicando (en este caso `R1`) tantas veces como el multiplicador indique (en este caso `R0`). Por ejemplo, para multiplicar 3 por 5, sumaríamos 5 tres veces: 5 + 5 + 5 = 15.

Aqui una pequeña explicacion del codigo
1. Se inicializa el registro `R2` en cero. Este registro se usará para acumular el resultado de la multiplicación.
2. Se copia el valor de `R0` (el multiplicador) en una variable llamada `count`.
3. Se establece un bucle etiquetado como `LOOP`. Este bucle repetirá las siguientes operaciones hasta que `count` llegue a cero:
   a. Se verifica si `count` es cero. Si lo es, el bucle termina y el programa salta a la etiqueta `END`.
   b. Se suma el valor de `R1` (el multiplicando) al valor acumulado en `R2`. Esto simula una multiplicación.
   c. Se decrementa `count` para seguir realizando la multiplicación el número de veces indicado por el multiplicador.
4. Después de salir del bucle, el programa entra en una sección etiquetada como `END`. Esto es simplemente un bucle infinito que detiene la ejecución del programa.

# FILL.ASM

El objetivo de Fill.asm es escribir una secuencia específica de comandos en el lenguaje de máquina del computador virtual, específicamente para llenar la pantalla con un patrón determinado. Este programa es parte de la fase de desarrollo del ensamblador, donde los estudiantes deben escribir un programa en lenguaje ensamblador que realizará una tarea específica, como llenar la pantalla con un patrón específico.

El propósito general de Fill.asm, como el de muchos programas de este tipo dentro del contexto del curso "From Nand to Tetris", es ayudar a los estudiantes a entender y practicar los conceptos de lenguaje de máquina, lenguaje ensamblador y arquitectura del computador, permitiéndoles construir gradualmente una pila de abstracciones que los llevarán desde el nivel más básico de hardware hasta un sistema informático completo y funcional.
