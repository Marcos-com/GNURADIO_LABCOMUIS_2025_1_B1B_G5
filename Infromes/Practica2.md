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


### Procedimiento
Debe basarse en las acciones efectivamente realizadas durante el laboratorio, describiendo los procesos realizados y los resultados obtenidos. Para cada práctica se pueden brindar preguntas orientadoras o pasos a seguir para establecer lo que se espera lograr/estudiar/analizar/obtener/comparar. Por ejemplo:
- Describa los procesos realizados en el laboratorio  y los resultados obtenidos.
- ¿Cómo se alcanza el límite de Nyquist y que pasa cuando se disminuye de este?
- ¿Por qué al interpolar una señal en GNURADIO su frecuencia disminuye?
- ¿Por qué al diezmar una señal en GNURADIO su frecuencia aumenta?
- ¿Cómo se puede determinar la frecuencia máxima de una señal desde lo experimental?
- ¿Qué le sucede a una señal de audio cuando no se respeta el teorema de Nyquist?
- Describa las funciones logradas con el Ecualizador desarrollado con GNURadio.

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
