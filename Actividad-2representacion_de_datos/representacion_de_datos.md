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

# Tipos de datos 

## 3.Actividad de Investigacion

# Tipos de Datos en Diferentes Lenguajes de Programación

Los lenguajes de programación manejan distintos tipos de datos para representar información como números, caracteres, cadenas de texto y valores booleanos. A continuación, se presenta una comparación de los principales tipos de datos en C, Java y Python.

## Tipos de Datos Comunes

### 1. **Números Enteros (Integer)**
Los números enteros representan valores sin parte decimal.

| Lenguaje | Tipo de Dato  | Abreviación |
|----------|--------------|-------------|
| C        | `int`        | `int`       |
| Java     | `int`        | `int`       |
| Python   | `int`        | `int`       |

### 2. **Números de Punto Flotante (Float/Double)**
Los números decimales se representan con punto flotante.

| Lenguaje | Tipo de Dato | Abreviación |
|----------|-------------|-------------|
| C        | `float`     | `float`     |
| C        | `double`    | `double`    |
| Java     | `float`     | `float`     |
| Java     | `double`    | `double`    |
| Python   | `float`     | `float`     |

### 3. **Caracteres (Character)**
Se utilizan para representar letras individuales.

| Lenguaje | Tipo de Dato | Abreviación |
|----------|-------------|-------------|
| C        | `char`      | `char`      |
| Java     | `char`      | `char`      |
| Python   | No tiene un tipo `char`, usa `str` con longitud 1 | `str` |

### 4. **Cadenas de Texto (String)**
Las cadenas de texto almacenan secuencias de caracteres.

| Lenguaje | Tipo de Dato | Abreviación |
|----------|-------------|-------------|
| C        | `char[]` (Arreglo de caracteres) | `char[]` |
| Java     | `String`    | `String`    |
| Python   | `str`       | `str`       |

### 5. **Booleanos (Boolean)**
Representan valores de verdad (`true` o `false`).

| Lenguaje | Tipo de Dato | Abreviación |
|----------|-------------|-------------|
| C        | `_Bool` (o `stdbool.h` para `bool`) | `_Bool` / `bool` |
| Java     | `boolean`   | `boolean`   |
| Python   | `bool`      | `bool`      |

### 6. **Otros Tipos de Datos**
Algunos lenguajes incluyen otros tipos de datos adicionales:

- **C:** `short`, `long`, `unsigned int`, `void`.
- **Java:** `byte`, `short`, `long`, `void`.
- **Python:** `complex` (para números complejos), `NoneType` (para valores nulos).

Cada lenguaje de programación define sus tipos de datos con nombres y características particulares. Mientras que C y Java requieren una declaración explícita del tipo de dato, Python usa una tipificación dinámica, lo que le permite determinar el tipo en tiempo de ejecución.

### 5.Organizacion de resultados

# Tipos de Datos en Diferentes Lenguajes de Programación

Los lenguajes de programación manejan distintos tipos de datos para representar información como números, caracteres, cadenas de texto y valores booleanos. A continuación, se presenta una comparación de los principales tipos de datos en C, Java y Python.

## Tabla Comparativa de Tipos de Datos

| Nombre de la Variable | Abreviación | Características Principales |
|----------------------|------------|----------------------------|
| Entero (Integer)    | `int`      | Valores enteros, sin parte decimal. Rango en C y Java depende del sistema (generalmente -2,147,483,648 a 2,147,483,647). En Python, el tamaño es dinámico. |
| Punto Flotante      | `float`    | Números con decimales, precisión simple (32 bits). En Python, es de precisión doble por defecto. |
| Doble Precisión     | `double`   | Similar a `float`, pero con mayor precisión (64 bits en C y Java). |
| Caracter            | `char`     | Representa un solo carácter en C y Java (8 bits en C, 16 bits en Java). En Python, se usa `str` con longitud 1. |
| Cadena de Texto     | `String` (Java), `char[]` (C), `str` (Python) | Secuencia de caracteres. En C, se usa un arreglo de `char`. En Java y Python, es un tipo de dato nativo. |
| Booleano           | `bool` (C/Python), `boolean` (Java) | Representa valores `true` o `false`. En C, requiere la librería `stdbool.h`. |
| Entero Largo       | `long`     | Variante de `int` con mayor capacidad. En Java es de 64 bits. |
| Entero Corto       | `short`    | Variante de `int` con menor capacidad, generalmente 16 bits. |
| Sin Signo          | `unsigned` | Solo números positivos. Se usa en C para `int`, `char`, `short`, `long`. |
| Números Complejos  | `complex`  | Solo en Python, representa números con parte real e imaginaria. |
| Valor Nulo         | `void` (C/Java), `NoneType` (Python) | Representa la ausencia de valor. `void` se usa para funciones sin retorno en C y Java. |

Cada lenguaje de programación define sus tipos de datos con nombres y características particulares. Mientras que C y Java requieren una declaración explícita del tipo de dato, Python usa una tipificación dinámica, lo que le permite determinar el tipo en tiempo de ejecución.

### 5.Ejercicio de Calculo de Espacio en Memoria


## Cálculo del Espacio en Memoria

Se almacena la siguiente información cada 10 segundos durante 24 horas:
- Un identificador numérico (entero)
- Una temperatura (punto flotante)
- Un valor lógico (booleano)
- Un texto de 10 caracteres

### **Tamaños de los datos (en C como referencia):**
| Tipo de Dato | Tamaño (bytes) |
|-------------|---------------|
| `int`       | 4 bytes       |
| `float`     | 4 bytes       |
| `bool`      | 1 byte        |
| `char[10]`  | 10 bytes      |

**Total por registro:**
4 + 4 + 1 + 10 = **19 bytes**

### **Cantidad de registros en 24 horas:**
Cada 10 segundos se almacena un registro, por lo que en 24 horas:
(24 × 60 × 60) / 10 = **8640 registros**

### **Espacio total requerido:**
8640 registros × 19 bytes = **164,160 bytes (aproximadamente 160.33 KB)**

El almacenamiento de los datos requeriría aproximadamente **160.33 KB** en memoria si se usan los tamaños de C como referencia. Este valor puede variar en otros lenguajes debido a diferencias en la representación de los tipos de datos.

### Conclusion.

La representación y almacenamiento de datos en computación se basa en el sistema binario, permitiendo manejar números, texto, imágenes y sonido de manera eficiente. Diferentes lenguajes como C, Java y Python ofrecen estructuras de datos con características específicas, influenciadas por la tipificación de cada uno. Gracias al trabajo de George Boole y su álgebra, hoy es posible procesar información digitalmente. Comprender estos conceptos es clave para optimizar el uso de memoria y desarrollar.
