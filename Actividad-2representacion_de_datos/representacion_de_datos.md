# Representación de Datos Digitales

1.Escribe un parrafó  explicando con tus propipias palabras, cómo se representa los datos en una computadora. Por ejemplo ¿cómo se ingresan números, letras, imágenes a una computadora?

Las computadoras trabajan con datos representados en formato binario (ceros y unos). A continuación, se explica cómo se representan diferentes tipos de datos:

### Representación de Números
Los números se representan en binario utilizando distintos sistemas:
- **Enteros sin signo**: Se usan directamente en binario.
- **Enteros con signo**: Se usa el complemento a dos.
- **Números decimales**: Se representan en coma flotante según el estándar IEEE 754.

Ejemplo de un número entero en binario:
```
Decimal: 5  ->  Binario: 101
```

### Representación de Letras y Caracteres
Los caracteres se representan mediante códigos como ASCII o Unicode.

Ejemplo:
- **Letra 'A' en ASCII**: 65 en decimal = `01000001` en binario.
- **Letra 'A' en Unicode (UTF-8)**: Igual a ASCII en este caso.

### Representación de Imágenes
Las imágenes se representan mediante píxeles, donde cada píxel tiene información de color:
- **Blanco y negro**: 1 bit por píxel (0=negro, 1=blanco).
- **Escala de grises**: Un byte por píxel (0-255).
- **Color**: Se usa RGB (rojo, verde, azul), donde cada canal tiene 8 bits (24 bits en total por píxel).

Ejemplo de código en Python para leer una imagen:
```python
from PIL import Image
img = Image.open('imagen.png')
img.show()
```

### Representación de Sonido
El sonido se digitaliza mediante muestreo y cuantificación:
- **Frecuencia de muestreo**: Cantidad de muestras por segundo (ej. 44.1 kHz para CD).
- **Profundidad de bits**: Bits usados para representar cada muestra (ej. 16 bits por muestra).

Ejemplo de onda sonora:
```
Analogico:  ~~~~~
Digital:    - - - - -
```

### Representación de Videos
El video es una secuencia de imágenes mostradas rápidamente (fps - cuadros por segundo), con audio sincronizado. Se comprime con algoritmos como H.264 o VP9.

### Entrada de Datos
Los datos ingresan a la computadora mediante dispositivos como:
- **Teclado** (caracteres ASCII/Unicode).
- **Ratón** (coordenadas y clics).
- **Escáner** (imágenes digitalizadas).
- **Micrófono** (señales de audio digitalizadas).

2.Luego de realizar el ejercicio 1, escribe tus conclusiones acerca de la pregunta planteada en la Figura 2. ¿Cuántos estados diferentes pueden ser representados por N variables binarias?

La cantidad de estados diferentes que pueden ser representados por N variables binarias es `2^N`. Esto se debe a que cada variable binaria puede tomar dos valores distintos (0 o 1), y con N variables, el número total de combinaciones posibles es `2^N`. Esta propiedad es fundamental en la computación, ya que permite representar una gran cantidad de información utilizando un número finito de bits.

3.¿Cuáles son las unidades de almacenamiento de datos que se utilizan en computación? Crea una tabla donde muestres estas unidades con sus prefijos. En este caso me refiero a KiloByte, MegaByte, etc. 
### Unidades de Almacenamiento de Datos
En computación, los datos se almacenan en distintas unidades de medida que utilizan prefijos estándar:

| Unidad       | Símbolo | Equivalencia en Bytes |
|-------------|---------|----------------------|
| Byte        | B       | 1 Byte               |
| KiloByte    | KB      | 1,024 Bytes          |
| MegaByte    | MB      | 1,024 KB             |
| GigaByte    | GB      | 1,024 MB             |
| TeraByte    | TB      | 1,024 GB             |
| PetaByte    | PB      | 1,024 TB             |
| ExaByte     | EB      | 1,024 PB             |
| ZettaByte   | ZB      | 1,024 EB             |
| YottaByte   | YB      | 1,024 ZB             |

4.Incluye un pequeño resumen, de un par de renglones, donde menciones la importancia del trabajo de George Bool en este tópico.
### Importancia del Trabajo de George Boole
El trabajo de George Boole en el álgebra booleana es fundamental para la representación y manipulación de datos en computación. Sus principios permiten la construcción de circuitos lógicos y la implementación de operaciones lógicas en los procesadores, lo que constituye la base del funcionamiento de las computadoras modernas.

---

# Actividad#2

### Convercion de binarios a decimales
- 1010101010<sub>2</sub> = 682<sub>10</sub>
- 11111<sub>2</sub> = 31<sub>10</sub>
- 10000000<sub></sub> = 128<sub>10</sub>
- 100100100<sub></sub> = 292<sub>10</sub>
- 111000<sub></sub> = 56<sub>10</sub>

## Ejercicio 2

### Convercion de decimal a binario
- 127<sub>10</sub> = 1111111<sub>2</sub>
- 246<sub>10</sub> = 11110110<sub>2</sub>
- 1025<zub>10</sub> = 10000000001<sub>2<sub>
- 354<sub>10</sub> = 101100010<sub>2</sub>
- 187<sub>10</sub> = 10111011<sub>2</sub>

