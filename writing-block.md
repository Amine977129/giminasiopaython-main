 Presentación oral – AC4  

## Gimnasio y Fitness



### 1. Introducción



Hola, buenos días.



Hoy voy a presentar mi práctica AC4, que consiste en analizar, limpiar y validar un conjunto de datos utilizando Python.



Mi conjunto de datos pertenece al sector de los gimnasios y el fitness.



El objetivo es detectar errores, limpiar los datos, separar los registros válidos de los rechazados y analizar los resultados.



### 2. Presentación del conjunto de datos



He trabajado con el archivo **giminasio.csv**, que contiene **120 registros iniciales**.



Cada registro representa un servicio, una cuota, una matrícula o una actividad relacionada con un centro deportivo.



Las columnas principales son:



**activitat**: nombre de la actividad o del servicio.
**tipus_activitat**: tipo de actividad o servicio.
**centre**: centro deportivo.
**participants**: número de participantes.
**durada_min**: duración en minutos.
**data**: fecha del registro.


Las variables numéricas son el número de participantes y la duración en minutos.



### 3. Relación entre AC3 y AC4



Para realizar esta práctica he seguido una estructura de trabajo similar a la de AC3.



He mantenido las fases principales: cargar y explorar los datos, detectar errores, limpiar y validar los registros, y analizar los datos válidos.



También he generado archivos de salida y un informe con los resultados. He adaptado el proceso a las columnas y a las características del sector de los gimnasios y el fitness.



### 4. Detección de problemas de calidad



Durante el análisis he detectado diferentes tipos de errores:



Campos obligatorios vacíos.
Números de participantes incorrectos, como valores negativos, decimales o textos.
Duraciones no válidas, como valores negativos, cero o textos.
Fechas incorrectas o inexistentes.
Espacios sobrantes en algunos campos de texto.


Por ejemplo, he encontrado **2,5 participantes** y una duración de **-12,5 minutos**. Estos valores no cumplen las reglas de validación.



### 5. Limpieza y validación



Para limpiar los datos he utilizado diferentes operaciones de Python.



He utilizado el método `strip()` para eliminar los espacios sobrantes al principio y al final de los textos.



También he comprobado que los campos obligatorios no estén vacíos, que los participantes sean números enteros positivos, que las duraciones sean numéricas y positivas, y que las fechas sean válidas.



En las duraciones, el programa también puede convertir la coma decimal en punto. Los registros que no cumplían las reglas fueron rechazados y sus incidencias quedaron registradas.



### 6. Generación de archivos y elaboración del informe



En la fase de generación de archivos, Python ha creado:



**registres_nets.csv**, con los registros válidos.
**incidencies.csv**, con los errores detectados.
**informe_resultats.txt**, con el resumen del análisis.


Para elaborar el informe he utilizado una cadena de texto con formato *f-string*, que permite incluir automáticamente los resultados.



También he utilizado `datetime.now()` para registrar la fecha y la hora de generación del informe. Finalmente, he guardado los archivos con codificación `utf-8-sig`.



### 7. Resultados del análisis



Después del proceso de limpieza, de los **120 registros iniciales**:



**90 registros fueron válidos**.
**30 registros fueron rechazados**.


Esto representa un **75 % de registros válidos** y un **25 % de registros rechazados**.



El total de participantes fue de **3.534**. La duración media por registro válido fue de **107,16 minutos**.



También he agrupado los participantes por tipo de actividad:



Cuota: **483**.
Entrenamiento personal: **908**.
Servicios: **734**.
Instalaciones: **782**.
Clase dirigida: **627**.


El entrenamiento personal presenta el valor más alto.



Por centros deportivos, los resultados fueron:



Girona: **779**.
Terrassa: **910**.
Tarragona: **486**.
Barcelona: **793**.
Mataró: **566**.


Terrassa presenta el valor más alto y Tarragona, el más bajo.



### 8. Conclusiones



Como conclusión, esta práctica me ha permitido aplicar un proceso de limpieza y validación a datos del sector de los gimnasios y el fitness.



He aprendido a detectar errores, aplicar reglas de validación, separar los registros válidos de los rechazados y generar archivos con los resultados.



También he comprendido que la calidad de los datos es fundamental para obtener resultados fiables.



Muchas gracias por vuestra atención. 