# PROYECTO 9 - ARQUITECTURA DE COMPUTADORES
# TicTacToe (Tres en Raya)
![Captura de pantalla 2024-04-25 213653](https://github.com/Fitman22/ArchiTech/assets/124414206/f2cdca71-a539-427a-8015-c93184487e76)

El juego del tres en raya en Jack se implementa utilizando varias clases y archivos de utilidades. He aquí un breve resumen de cada archivo:

**TicTacToeGame.jack:** Esta clase es el controlador principal del juego. Inicializa el juego, maneja la entrada del usuario, y gestiona el bucle de juego. Utiliza las clases Board, Piece, InputUtil y Random para implementar la lógica del juego.

**Random.jack:** Esta clase proporciona métodos para generar números aleatorios. Se utiliza en la clase TicTacToeGame para seleccionar aleatoriamente el primer jugador.

**Piece.jack:** Esta clase representa las piezas del juego (X o O). Tiene atributos para el tipo de pieza, anchura y altura. La clase proporciona métodos para dibujar las piezas y obtener su tipo.

**Main.jack:** Esta clase es el punto de entrada del juego. Inicializa el juego e inicia el bucle de juego. Utiliza la clase TicTacToeGame para gestionar el juego.

**InputUtil.jack:** Esta clase proporciona métodos para manejar la entrada del usuario. Se utiliza en la clase TicTacToeGame para obtener la entrada del usuario y manejar los eventos del juego.

**Board.jack:** Esta clase representa el tablero de juego y gestiona el estado del juego. Tiene atributos para las dimensiones del tablero, la matriz del tablero, y las banderas para las condiciones de ganar y empatar. La clase proporciona métodos para crear un nuevo tablero, limpiar el tablero, evaluar el estado del tablero, y manejar movimientos y empates.

El juego comienza creando un nuevo objeto Tablero e inicializando las piezas del juego. A continuación, el jugador realiza movimientos seleccionando una casilla vacía del tablero. El estado del juego se evalúa después de cada movimiento, y si hay un ganador o un empate, el juego termina. El juego también se puede terminar pulsando la tecla «0».


# Desarrolle más el concepto de lenguaje de alto nivel, teniendo en cuenta la diferencia entre lenguajes de programación propiamente dichos e interpretadores.

Hace varios años programar era una cosa, cuando menos, problemática. Hoy en día tenemos las herramientas para usar nuestro lenguaje y que esta sea entendido por el computador. Y es que esto no es nada sencillo, como tal los computadores no entienden nuestro lenguaje, ellos solo comprenden cadenas de bites (0’s y 1’s). 

De allí viene el uso de los lenguajes de programación de alto nivel, el cual es un lenguaje de programación diseñado para que sea fácil de leer y escribir para las personas. Esta es su principal diferencia con los lenguajes de bajo nivel, como por ejemplo el ensamblador, que están más cerca del lenguaje de la máquina.

Hay un error muy común que comenten las personas en esta área, y es de afirmar que los intérpretes y los leguajes de alto nivel son lo mismo. Los lenguajes de programación propiamente dichos son aquellos que permiten a los programadores escribir instrucciones para realizar tareas específicas. Estos lenguajes se utilizan para crear programas y aplicaciones que pueden realizar una amplia variedad de funciones, desde procesamiento de texto hasta cálculos complejos y gestión de bases de datos.

Por otro lado, un intérprete es un programa que ejecuta instrucciones escritas en un lenguaje de programación de alto nivel. Toma el código fuente escrito por el programador y lo convierte en instrucciones que la computadora puede entender y ejecutar directamente. En lugar de compilar todo el código a lenguaje de máquina de una vez, como lo hace un compilador, el intérprete interpreta y ejecuta cada línea de código una por una en tiempo real.

La principal diferencia entre un lenguaje de programación y un intérprete radica en cómo se ejecuta el código. Con un lenguaje de programación, el código se traduce en un archivo ejecutable que puede ser ejecutado directamente por la computadora. Con un intérprete, el código se interpreta y ejecuta línea por línea, lo que proporciona una mayor flexibilidad y facilidad de depuración, pero a menudo a expensas de la velocidad de ejecución.


# ¿Qué lenguajes interpretadores ademas del Python existen?
  # JavaScript:
  Ampliamente utilizado en el desarrollo web para la creación de aplicaciones interactivas en el lado del cliente y del servidor.
  # Ruby: 
  Conocido por su elegancia y facilidad de uso, es especialmente popular en el desarrollo web, especialmente con el framework Ruby on Rails.
  # PHP: 
  Ampliamente utilizado en el desarrollo web para la creación de páginas dinámicas y aplicaciones web.
  # Perl: 
  Conocido por su capacidad para procesar texto de manera eficiente, es utilizado en una variedad de aplicaciones, desde la administración de sistemas hasta el desarrollo web.
  # Lua: 
  Utilizado principalmente en aplicaciones que requieren scripting, juegos y desarrollo de software embebido.
  # Shell Scripting (Bash, etc.): 
  Ampliamente utilizado en sistemas Unix y Linux para la automatización de tareas y la administración del sistema.
  # R: 
  Utilizado en estadísticas y análisis de datos, es especialmente popular en la comunidad académica y de investigación.
  # MATLAB: 
  Utilizado en aplicaciones de computación numérica y técnica, es comúnmente utilizado en ingeniería y ciencias aplicadas.

# Bonus: ¿Qué se debe considerar para proponer un nuevo y buen lenguaje de programación, teniendo en cuenta la arquitectura de computador completa? Justifique su respuesta.

Proponer un nuevo y buen lenguaje de programación teniendo en cuenta la arquitectura completa de computadoras implica considerar varios aspectos importantes para asegurar su utilidad, eficiencia y aceptación en la comunidad de desarrollo como:

Eficiencia y rendimiento: El lenguaje debe permitir la escritura de código eficiente que pueda ejecutarse de manera rápida y utilizar eficazmente los recursos del sistema, como la memoria y la CPU.

Seguridad: El lenguaje debe incluir características que ayuden a prevenir vulnerabilidades de seguridad, como la gestión segura de la memoria y la detección de errores en tiempo de compilación.

Portabilidad: Debería ser posible ejecutar programas escritos en el lenguaje en una variedad de plataformas y arquitecturas de hardware sin modificaciones significativas.

Modelo de memoria: El lenguaje debe tener características que permitan un manejo eficiente de la memoria, teniendo en cuenta la jerarquía de memoria del sistema (caché, RAM, disco). Un buen lenguaje minimiza el uso de la memoria y proporciona herramientas para gestionar la asignación y liberación de memoria de manera segura y eficiente.

Modelo de concurrencia: La arquitectura del hardware influye en cómo se pueden diseñar y ejecutar programas concurrentes de manera eficiente. El lenguaje debería ofrecer abstracciones y herramientas que faciliten la programación concurrente y paralela, aprovechando las características del hardware como múltiples núcleos de CPU.

Instrucciones y conjuntos de instrucciones: Es importante considerar cómo el lenguaje interactuará con el conjunto de instrucciones subyacente del procesador. Un buen lenguaje puede proporcionar abstracciones que permitan a los programadores escribir código de manera independiente del conjunto de instrucciones específico, pero también puede permitir la optimización manual cuando sea necesario.

Estructuras de datos y alineación de memoria: El lenguaje debe permitir la definición de estructuras de datos eficientes que se alineen adecuadamente en la memoria para minimizar la fragmentación y maximizar el rendimiento del acceso a los datos.

Gestión de recursos: Debe haber soporte en el lenguaje para la gestión eficiente de recursos de hardware, como archivos, dispositivos de red y periféricos. Esto implica proporcionar mecanismos para abrir, cerrar y manipular recursos de manera segura y eficiente.

Optimización de código: El lenguaje debe permitir la optimización del código para aprovechar las características específicas del hardware, como las instrucciones SIMD (Single Instruction, Multiple Data) o las capacidades de paralelización del procesador.

