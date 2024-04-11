# PROYECTO #7 - ARQUITECTURA DE COMPUTADORES
Máquina Virtual

Introducción:
El proyecto busca desarrollar un 'traductor' que convierta los comandos de programas escritos en lenguaje VM a una secuencia de comandos en lenguaje hack. El objetivo es que estos programas realicen las mismas tareas que los archivos de comparación proporcionados por el sitio de Nand2Tetris.

El desarrollo del proyecto se divide en dos etapas: una primera fase que se centra en traducir los comandos aritméticos de pila y los comandos de acceso a la memoria, y una segunda fase que amplía la traducción a los comandos de llamada de funciones y bifurcaciones del lenguaje VM.

Desarrollo Proyecto 7:
En este proyecto, se desarrolla una máquina virtual crucial para la traducción de código de alto nivel a bajo nivel, utilizando Python y principios de programación orientada a objetos.

La estructura de la máquina virtual comprende dos clases principales: "Parser" y "CodeWriter."

La clase "Parser" prepara el archivo de entrada eliminando comentarios y espacios innecesarios. Identifica el tipo de comando y proporciona información adicional como argumentos.

La clase "CodeWriter" configura el convertidor de código para el archivo de salida y escribe los comandos aritméticos y de "push" y "pop" según corresponda.

