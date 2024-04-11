# PROYECTO #8 - ARQUITECTURA DE COMPUTADORES
Desarrollo Proyecto 8:
Este proyecto extiende el Proyecto 7 con nuevos comandos VM como "label," "goto," "if-goto," "function," "call," y "return."

Se agregan funciones específicas en la clase "CodeWriter" para manejar estos nuevos comandos y se incorpora una función para escribir el código bootstrap de VM.

El proceso de traducción se realiza de manera similar al proyecto anterior, con ajustes para manejar los nuevos comandos.

# Futuro de las Máquinas Virtuales:
Las máquinas virtuales enfrentan desafíos en rendimiento, seguridad, compatibilidad y gestión de recursos, pero su futuro se ve prometedor.

Tendencias como la integración con la inteligencia artificial y la computación cuántica, mejoras en el hipervisor, y la expansión de la nube y el edge computing, podrían influir en su evolución.

La integración con tecnologías avanzadas y el desarrollo continuo del software apuntan hacia una administración más eficaz y segura de las máquinas virtuales.

# Cuál es la principal similitud entre un contenedor y una máquina virtual?
Una de las similitudes más notables entre los contenedores y las máquinas virtuales es su capacidad para proporcionar entornos de ejecución aislados y portátiles. Tanto los contenedores como las máquinas virtuales permiten encapsular las aplicaciones y sus dependencias en un entorno virtual, haciéndolas independientes del sistema operativo y del hardware subyacente. Esta característica es esencial para implementar soluciones de computación en la nube donde la portabilidad y la escalabilidad son esenciales. Además, tanto los contenedores como las máquinas virtuales brindan soluciones eficientes para la gestión de recursos y la distribución de cargas de trabajo en entornos de infraestructura de TI. Ambos permiten que se ejecuten múltiples aplicaciones en un único servidor físico, maximizando la utilización de recursos y simplificando la administración y la implementación de aplicaciones.
# ¿Cual es la ventaja del contenedor respecto a la máquina virtual?
Una de las ventajas radica en su eficiencia y velocidad. Los contenedores comparten el kernel del sistema operativo del host, eliminando la necesidad de ejecutar múltiples sistemas operativos completos como en el caso de las máquinas virtuales. Esto reduce significativamente los requisitos de recursos y el tiempo de inicio de los contenedores en comparación con las máquinas virtuales. Además, los contenedores son más livianos al evitar la sobrecarga asociada con la emulación de hardware de una máquina virtual, lo que los hace ideales para despliegues a gran escala y aplicaciones que requieren alta movilidad y flexibilidad. Otra ventaja importante es su portabilidad, ya que encapsulan no solo la aplicación, sino también todas sus dependencias y bibliotecas necesarias para su ejecución, garantizando que se ejecute de manera consistente en cualquier entorno que admita contenedores, independientemente del sistema operativo utilizado.