# PROYECTO 4 - ARQUITECTURA DE COMPUTADORES

# MULT.ASM

**Mult.asm** es un archivo de código escrito en lenguaje ensamblador para el proyecto **04** del curso **Nand2Tetris**. El objetivo principal de este programa es realizar la multiplicación de los valores almacenados en los registros **R0** y **R1**, y luego guardar el resultado en el registro **R2**.

En términos más sencillos:
- **Entrada**: Los valores iniciales se encuentran en los registros **R0** y **R1**.
- **Proceso**: El programa realiza la multiplicación de estos valores.
- **Salida**: El resultado se almacena en el registro **R2**.

El código se divide en las siguientes partes:
1. **Inicialización**: Se establece el valor inicial del registro **R2** en cero.
2. **Verificación de productos cero**: Se verifica si alguno de los valores en **R0** o **R1** es cero. Si es así, el programa salta al punto de finalización.
3. **Bucle de multiplicación**: Si ambos valores son distintos de cero, el programa entra en un bucle de multiplicación. En cada iteración, suma el valor actual en **R1** al valor en **R2** y decrementa un contador en **R3**.
4. **Finalización del programa**: Una vez que el contador en **R3** llega a cero o es negativo, el programa finaliza.

Esencialmente, **Mult.asm** es un ejemplo simple de cómo se realiza la multiplicación en lenguaje ensamblador. Puedes encontrar el código completo en el [repositorio de GitHub](https://github.com/adeosd16/mult.asm) .
