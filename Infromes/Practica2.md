# Laboratorio de Comunicaciones
## Universidad Industrial de Santander

# Práctica 1:  MODELO DE CANAL

### Integrantes
- **MARCOS DAVID ARRIETA BARRETO** - 2204657
- **SEGUNDO INTEGRANTE** - Código

Escuela de Ingenierías Eléctrica, Electrónica y de Telecomunicaciones  
Universidad Industrial de Santander

### Fecha
20 de Marzo de 2025

---

## Declaración de Originalidad y Responsabilidad
Los autores de este informe certifican que el contenido aquí presentado es original y ha sido elaborado de manera independiente. Se han utilizado fuentes externas únicamente como referencia y han sido debidamente citadas.

Asimismo, los autores asumen plena responsabilidad por la información contenida en este documento. 

Uso de IA: [Indicar si se usó IA y para qué aspectos específicos, por ejemplo: "Se utilizó ChatGPT para reformular secciones del texto y verificar gramática, pero el contenido técnico fue desarrollado íntegramente por los autores."]

---
## Contenido

### Resumen
En esta práctica, analizamos y aprendimos cómo la calidad de una señal puede variar dependiendo del tipo de canal a través del cual se transmite. Para ello, observamos la señal en el osciloscopio y en el analizador de espectro. También investigamos cómo mitigar los efectos que el canal puede producir en la señal.

Además, analizamos la relación señal a ruido para determinar qué componente predomina en cada canal. Finalmente, comparamos los diferentes tipos de canales para evaluar cuál es más eficiente en la transmisión de datos y cuál mantiene la mejor calidad de la señal.

### Introducción
- ¿Cuál es el efecto de filtrar las frecuencias altas de una señal?

  Cuando nosotros eliminamos las frecuencias altas de una señal lo que estamos provocando es eliminando los armonicos de la señal lo que provocaria que se queden solo el fundamental y la señal se convierte en una onda senoidal.
- ¿Qué sucede al filtrar muy cerca de la frecuencia fundamental de la señal?

  Al filtar cerca de la frecuencia fundamental la señal de salida podria presentar o comportarse como una señal ruidosa, y si eliminamos por completo todos los armonicos y el fundamental eliminariamos la señal completa.
- ¿Cuál es el efecto de filtrar las frecuencias bajas de una señal?

  El efecto que provocaria eliminar las frecuencias bajas puede provocar discontinuidad en la señal esto se puede ver como picos o pulsos, generando cambios rapidos en la señal.
- ¿Qué ocurre al eliminar armónicos de una señal?

  Cuando eliminamos los armonicos de la señal es decir el fundamental y todos los demas lo que provocamos es eliminar o atenuar la señal, lo que provocaria perdida total de la señal.
- ¿Qué efecto tiene la desviación de frecuencia en la señal recibida? ¿Qué efecto(s) produce el filtro cuando la señal recibida se ve afectada por desviación de frecuencia?

  Cuando recibimos la señal con una desviacion de frecuencia esto puede provocar que el receptor pueda sintonixar o leer mal la señal, tamien puede llegar el caso de perderla, y cuando pasa por un filtro va depender del filtrado que se aplique puede provocar diferentes tipos de consecuencias.
- ¿Cómo cuantificar la degradación de la señal al aumentar los niveles de ruido?

  Para cuantificar la señal, para ver que tanto afecta el ruido, dedemos irnos a la relacion señal a ruido, esta no podra decir que tanto afecta la potencia del ruido a la potencia de la señal, cuando esta es alta podemos obtener una mejor calidad de señal, pero cuando esta es baja, quiere decir que la potencia del ruido es mucho mas alta, y no tendra mucha calidad la señal.
- ¿Cómo se puede mejorar la relación señal a ruido en una señal?

  Para mejorar la relacion señal a ruido, hay muchos metodos, uno de ellos pude ser aumentando la potencia de la señal y disminuyendo la potencia del ruido, esto provocaria una mejor calidad de la señal.

### Procedimiento
Ahora vamos a dar seguimiento a las actividades 2 y 3, es cuando veremos en la parte experimental de como podemos notar tanto en el osciloscopio y en el analixador de espectro los efectos de canal. Resolviendo las siguintes preguntas orientadoras:

- ¿Cuál es el efecto del ruido sobre la amplitud de las señales medidas en el osciloscopio? ¿Conservan las mismas relaciones que se evidencian en la simulación?
  El efecto que provoca el ruido a la amplitud de la señal se puede ver un aumento considerable ya como nos muestra los cursores del osciloscopio. como se puede ver a continuacion.
  SEÑAL SIN RUIDO
  ![Señal sin ruido](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/Se%C3%B1al%20sin%20ruido.jpg)
  SEÑAL CON RUIDO
  ![Señal con ruido](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/Se%C3%B1al%20con%20ruido.jpg)  
- ¿La relación señal a ruido creada intencionalmente en el computador se amplifica o se reduce en la señal observada en el osciloscopio?

  Aumenta esto podemos nortarlo, ya que cada vez que que nosotros variamos el ruido, podemos ver que la relacion señal a ruido aumenta ya que la señal va perdiendo calidad como se muestra en la siguiente imagen con diferentes niveles de ruido de 0.03 y de 0.09.
  SEÑAL CON RUIDO DE 0.03
  ![Señal con ruido de 0.03](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/Se%C3%B1al%20con%200.3%20de%20ruido.jpg)
  SEÑAL CON RUIDO DE 0.09
  ![Señal con ruido de 0.09](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/Se%C3%B1al%20con%200.09%20de%20ruido.jpg)  
- Demuestre ¿cómo se puede mejorar la relación señal a ruido en una señal?

  Una forma de mejorr la relacion señal a ruido es mejorar o aumental la potencia del trasmisor, esto provocaria que la relacion señal a ruido aumentara y asi mismo su calidad, o buscando un cable que no tenga tanta atenuacion.
- ¿Cómo se evidencia el fenómeno de desviación de frecuencia en el osciloscopio? Evidenciar al menos con dos formas de onda.
  Para ver la desviacion de frecuencia podemos notarlo mediante la frecuencias, ya que esta se desfasaria y y pierde la frecuencia que originalmente tendria como se puede ver en las siguientes imagenes.
  SEÑAL SIN DESVIACION
  ![Señal sin desviacion](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/sin%20desviasion.jpg)
  SEÑAL CON DESVIACION
  ![Señal con desviacion](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/con%20desviacion.jpg)
- Determine la afectación de un medio de transmisión coaxial (usar cables largos) sobre una señal periódica operando a las capacidades máximas de muestreo del USRP.

  Usar los cables largos (coaxiales) esto porvoca que pueda ver mas atenuacion de la señal y se puede notar en el osciloscopio, ya que vemos la señal, mas pequeña, como se muestra en la imagen.
  CON CABLE COAXIAL
  ![Señal con cable coaxial](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/cable%20coaxial.jpg)
- Usando antenas, ¿cómo afecta la distancia entre el transmisor y el receptor a la amplitud de la señal medida? ¿Es posible compensar el fenómeno?

  La distancia afecta muy considerablemente la amplitud de la señal ya que esta puede propagarse en el aire o objetos que se encuentran en el medio puede que pierda energia. lo podemos ver en la siguientes imagenes.
  SEÑAL CON ANTENAS JUNTAS
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/con%20antenas%20juntas.jpg)
  SEÑAL CON ANTENAS SEPARADAS
  ![Señal con antenas separadas](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/antenas%20repadas.jpg)
- ¿Qué modelo de canal básico describe mejor las mediciones obtenidas en la práctica?

  El mejor canal es el cable corto, ya que no presenta tantas atenuaciones como los otros canales por ejemplo el cable coaxial su largor puede que presente mas atenuacion, las antenas pueden pueden perder energia ya que el ambiente y algunos objetos pueden hacer interferir.

Ahora veremos las preguntas orientadoras de la actividad 3 y sus observaciones:
- ¿Cuál es el efecto del ruido sobre la respuesta en frecuencia de las señales medidas en el analizador de espectro? ¿Conservan las mismas relaciones que se evidencian en la simulación?
  El efecto mas evidente es el piso de ruido aumenta o disminuye dependiendo de cuanto ruido mandamos, se pude notar mucho mejor en las imagenes y podemos ver que la comparacion entre la simulacion y lo real mantienen un margen de error muy pequeño esto puede ser por como esta configurado el analizador de espectros.
  SIMULACION
    ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/con%20ruido.jpg)
  ANALIZADOR DE ESPECTROS
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20con%20ruido.jpg)
  Podemos ver la diferencia de las señales sin ruido que tienen un ruidode piso muy bajo.
  SIMULACION SIN RUIDO
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/sin%20ruido.jpg)
  ANALIZADOR DE ESPECTROS SIN RUIDO
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20sin%20ruido.jpg)
- ¿La relación señal a ruido creada intencionalmente desde el computador se amplifica o se reduce en la señal observada en el analizador de espectro?

  Podemos ver que el ruido creado por el computador se amplifica  cuando nosotros subimos o aumentamos el ruido, podemos verlo como el piso de ruido aumenta en el analizador de espectros y comparando con la señal sin ruido de cada señal.
    SIMULACION SIN RUIDO(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/sin%20ruido.jpg)
  ANALIZADOR DE ESPECTROS SIN RUIDO(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20sin%20ruido.jpg)
  SIMULACION SIN RUIDO(ONDA CUADRADA)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/se%C3%B1al%20cuadrada.jpg)
  ANALIZADOR DE ESPECTROS SIN RUIDO(ONDA CUADRADA)
  ![Señal con antenas cerca](http://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20con%20una%20cuadra.jpg)
  Aplicamos varios valores de ruido para ver si el analizador de espectro se puede notar los diferentes tipos niveles de ruido.
  
    SIMULACION CON RUIDO DE 0.8(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/con%20ruido%20de%200.8.jpg)
  ANALIZADOR DE ESPECTROS CON RUIDO DE 0.8(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20con%20ruido%20de%200.8.jpg)
    SIMULACION CON RUIDO DE 0.16(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/con%20ruido%20de%200.16.jpg)
  ANALIZADOR DE ESPECTROS CON RUIDO DE 0.16(ONDA SENO)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20con%20ruido%20de%200.16.jpg)
  SIMULACION CON RUIDO DE 0.4(ONDA CUADRADA)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/cuadrada%20con%20ruido%20de%200.4.jpg)
  ANALIZADOR DE ESPECTROS CON RUIDO DE 0.4(ONDA CUADRADA)
  ![Señal con antenas cerca](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2C/espectro%20de%20cuadrada%20con%20ruido%20de%200.4.jpg)
- ¿Cómo se evidencia el fenómeno de desviación de frecuencia en el analizador de espectro? Evidenciar al menos con dos formas de onda.

  Para evidenciar la desviacion de frecuencia podemos ver que la frecuencia central se desplaza, y podemos verlo tanto en la simulacion como en el analizador de espectros.
  
- Determine la afectación de un medio de transmisión coaxial (usar cables largos) sobre una señal periódica operando a las capacidades máximas de muestreo del USRP.
- Usando cables coaxiales de diferentes longitudes, ¿cómo afecta la distancia entre el transmisor y el receptor a la amplitud de la señal medida?
- Usando antenas, ¿cómo afecta la distancia entre el transmisor y el receptor a la amplitud de la señal medida? ¿Es posible compensar el fenómeno?
- ¿Qué modelo de canal básico describe mejor las mediciones obtenidas en la práctica?
### Conclusiones
Se sintetizan los principales aportes y puntos relevantes de la práctica, evitando repetir lo ya consignado en las otras secciones del informe. 

### Referencias
Ejemplo de referencia:

- [Proakis, 2014] J. Proakis, M. Salehi. Fundamentals of communication systems. 2 ed. England: Pearson Education Limited, 2014. p. 164-165, 346. Chapter 5 In: [Biblioteca UIS](https://uis.primo.exlibrisgroup.com/permalink/57UIDS_INST/63p0of/cdi_askewsholts_vlebooks_9781292015699)

---
# Ejemplos usando Markdown

Volver al [INICIO](#laboratorio-de-comunicaciones)

## Inclusión de Imágenes
### Imagen de referencia dentro del repositorio:
![Networking](my%20file/test.png)

### Imagen de fuente externa
![GNU Radio logo](https://github.com/Marcos-com/GNURADIO_LABCOMUIS_2025_1_B1B_G5/blob/main/Practica_2/Practica_2B/Se%C3%B1al%20sin%20ruido.jpg)

### Uso de html para cambiar escala de la imagen
<img src="https://kb.ettus.com/images/thumb/5/50/gnuradio.png/600px-gnuradio.png" alt="GNU Radio Logo" width="300">

## Creación de hipevínculos 
- [Aprende Markdown](https://markdown.es/)
- [Más acerca de Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Abrir documento en el repositorio](my%20file/test_file.txt). Si hay espacios en la ruta de su archivo, reemplácelos por `%20`.
- Ir a una sección de este documento. Por ejemplo: [Ir a Contenido](#contenido) Tenga en cuenta escribir el título de la sección en minúsculas y los espacios reemplazarlos por guiones.
## Uso de Expresiones Matemáticas
Se pueden incluir ecuaciones en el archivo `README.md` utilizando sintaxis similar a [LaTeX](https://manualdelatex.com/tutoriales/ecuaciones):

### Ecuaciones en Línea
```
La energía de una señal exponencial es $E = \int_0^\infty A^2 e^{-2t/\tau} dt$.
```
**Salida renderizada:**
La energía de una señal exponencial es $E = \int_0^\infty A^2 e^{-2t/\tau} dt$.

### Ecuaciones en Bloque
```
$$E = \int_0^\infty A^2 e^{-2t/\tau} dt = \frac{A^2 \tau}{2}$$
```
**Salida renderizada**
$$E = \int_0^\infty A^2 e^{-2t/\tau} dt = \frac{A^2 \tau}{2}$$

## Creación de Tablas

**Tabla 1.** Ejemplo de tabla en Markdown.

| Parámetro | Valor |
|-----------|-------|
| Frecuencia (Hz) | 1000 |
| Amplitud (V) | 5 |
| Ciclo útil (%) | 50 |

## Inclusión de código

```python
def hello_world():
    print("Hello, World!")
```

También es posible resaltar texto tipo código como `print("Hello, World!")`.

---

Volver al [INICIO](#laboratorio-de-comunicaciones)
