# Instituto Tecnológico de Costa Rica
 
# Escuela de Computación 

# Estructuras de Datos Proyecto # 1

# Profesor Armado Arce Orozco

# Estudiantes : Michael Montano Bermúdez 
#               Gabriel Barrantes Rodas
# Documentación
### Introducción
   El objetivo de este proyecto es la lectura y despliegue de archivos tipo shapefile, leídos en su respectiva conversión a ascii, utilizando el lenguaje C++ se realizara la implementación de las funcionalidades de leer, dibujar, zoom al área observada, tanto acercamiento como alejamiento.
   Para el manejo de gráficos se utilizara la libreria FLTK para C++ que permite dibujar líneas, rectángulos, y cualquier otra figura geométrica, rellenar estas figuras con colores sólidos o gradientes y texturas etc.
   La lectura se podra hacer desde un archivo tipo shapefile convertido a formato ascii convertido por la aplicación Shpdump.
   
### Contenido a desplegar 
   El contenido a desplegar puede ser cualquier información contenida en un shapefile en formato ascii, que puede ser desde calles hasta figuras geométricas o indicadores de población por ejemplo.
   
### Estructuras de Datos utilizadas
   
### Algoritmo Ramer Douglas Peucker 
   
   La curva de partida es un conjunto ordenado de puntos o líneas y la dimensión distancia e> 0.
   
   El algoritmo recursivamente divide la línea. Inicialmente se administra todos los puntos entre el primer punto y el último. Marca automáticamente el primer y último punto que se le mantenga. A continuación, encuentra el punto que está más alejado del segmento de línea con los puntos primero y último como puntos finales (este punto es obviamente más lejos en la curva desde el segmento de línea aproximación entre los puntos finales). Si el punto está más cerca de e desde el segmento de línea entonces los puntos marcados en la actualidad no se puede mantiene y son descartados.
   
   Si el punto más alejado del segmento de línea es mayor que e en la aproximación siguiente debe ser mantenido. El algoritmo de forma recursiva llama a sí mismo con el primer punto el punto mas alejado y luego con el mas alejado y el último punto (que incluye marcado el peor punto de ser marcado como mantenido).
Cuando la repetición se completa una nueva curva de salida puede generarse integrado por todos aquellos puntos que han sido marcados como guardados.
   
### Forma de compilación 
   La forma de compilación es mediante el uso de un compilador para el lenguaje C++, no se requiere ningún trato especial.
   
### Limitaciones Observadas Posibles mejoras
   No se dio un uso al algoritmo de simplificación, no se da una simplificación de las lineas de forma adecuada.