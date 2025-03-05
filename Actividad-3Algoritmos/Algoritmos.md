# Algoritmos

## Ejercicio 1.
**Simbolos que se utilizan para representar operacioness de algoritmos con diagrama de flujo**

En los diagramas de flujo, se utilizan símbolos gráficos estandarizados para representar cada operación de un algoritmo. Estos permiten visualizar la secuencia lógica de un proceso de manera clara y estructurada. A continuación, s

- Óvalo (Inicio/Fin) : Se emplea par
- Paralelogramo (Entrada/Salida) : Se usa para representar la en
- Rectángulo (Proceso) : I
- Rombo (Decisión) : Repre
- Flechas (Líneas de flujo) : Conect
- Círculo (Conector) : Se u

El uso adecuado de estos símbolos permite representar algoritmos  de forma organizada y comprensible, facilitando su análisis y corrección.

[Simbolos para representar operaciones de algoritmos con diagrama de flujos](https://www.smartdraw.com/flowchart/simbolos-de-diagramas-de-flujo.htm?srsltid=AfmBOoqEA_Eipu1dG0-jsND9IbKjTmPbiJMqCZgcTHpm_a5ThPcDF5Ae)

## Ejercicio 2. 
### Pseudocódigo para calcular ingreso total semestral y promedio mensual.

Inicio

    Escribir "Ingrese el ID del empleado:"
    Leer ID_Empleado
    Escribir "Ingrese los seis sueldos del empleado:"
    Leer sueldo1, sueldo2, sueldo3, sueldo4, sueldo5, sueldo6

    ingreso_total <- sueldo1 + sueldo2 + sueldo3 + sueldo4 + sueldo5 + sueldo6
    promedio_mensual <- ingreso_total / 6

    Escribir "ID del Empleado: ", ID_Empleado
    Escribir "Ingreso Total Semestral: ", ingreso_total
    Escribir "Promedio Mensual: ", promedio_mensual
Fin

## Ejerccicos.

### 1.

# Algoritmo para calcular el costo de lápices.

## Pseudocódigo.
```plaintext
Inicio
    Escribir "Ingrese la cantidad de lápices:"
    Leer cantidad
    
    Si cantidad >= 1000 Entonces
        precio <- 85
    Sino
        precio <- 90
    FinSi
    
    total <- cantidad * precio
    
    Escribir "El costo total a pagar es: ", total
Fin
```
## Diagrama de flujo.

![alt text](imagenes/lapiz_diagrama.png)

### 2.

# Algoritmo para calcular el precio final con descuento en un almacén de ropa.


## Pseudocódigo.
```plaintext
Inicio
    Escribir "Ingrese el monto total de la compra:"
    Leer monto_compra
    
    Si monto_compra > 250000 Entonces
        descuento <- monto_compra * 0.15
    Sino
        descuento <- monto_compra * 0.08
    FinSi
    
    precio_final <- monto_compra - descuento
    
    Escribir "El descuento aplicado es: ", descuento
    Escribir "El precio final a pagar es: ", precio_final
Fin
```

## Diagrama de flujo.

![alt text](<imagenes/Diagrama_de _flujo.png>)

### 3.

# Algoritmo para calcular el costo del viaje de estudios.

## Pseudocódigo.
```plaintext
Inicio
    Escribir "Ingrese la cantidad de alumnos que asistirán al viaje:"
    Leer cantidad_alumnos
    
    Si cantidad_alumnos >= 100 Entonces
        costo_por_alumno <- 65
        total_pagar <- cantidad_alumnos * costo_por_alumno
    Sino Si cantidad_alumnos >= 50 Entonces
        costo_por_alumno <- 70
        total_pagar <- cantidad_alumnos * costo_por_alumno
    Sino Si cantidad_alumnos >= 30 Entonces
        costo_por_alumno <- 95
        total_pagar <- cantidad_alumnos * costo_por_alumno
    Sino
        total_pagar <- 4000
        costo_por_alumno <- total_pagar / cantidad_alumnos
    FinSi
    
    Escribir "El costo por alumno es: ", costo_por_alumno
    Escribir "El total a pagar a la compañía de viajes es: ", total_pagar
Fin
```

## Diagrama de flujo.

![alt text](imagenes/diagrama_de_flujo.png)

---

# Identificar Algoritmos. 

1. **Una página web**  
   **No representa un algoritmo.** Una página web es una estructura de información que muestra contenido (texto, imágenes, videos, etc.), pero no necesariamente sigue una secuencia definida de pasos para resolver un problema.

2. **Una receta para hacer un pastel, donde se indican ingredientes y pasos a seguir.**  
   **Sí representa un algoritmo.** Contiene una serie de pasos bien definidos que, si se siguen en orden, conducen a un resultado específico (el pastel).

3. **"Piensa en un número y multiplícalo por otro".**  
   **No representa un algoritmo.** Aunque sugiere una operación matemática, no define claramente un conjunto de pasos sistemáticos, ni un resultado concreto.

4. **Un manual de instrucciones para armar un mueble, con pasos detallados y un orden claro.**  
   **Sí representa un algoritmo.** Presenta una secuencia ordenada de pasos que llevan a un objetivo específico (armar el mueble), con instrucciones claras y sistemáticas.

5. **Una lista de compras organizada en orden alfabético.**  
   **No representa un algoritmo.** Es simplemente una colección de elementos sin una secuencia de pasos que conduzcan a una solución o a la resolución de un problema.

---

# Variables y constantes.

1. **El valor de la gravedad en la Tierra, 9.8 m/s².**  
   **Es una constante.** Porque su valor no cambia en condiciones normales.

2. **La edad de una persona calculada con base en el año actual y su año de nacimiento.**  
   **Es una variable.** Porque cambia con el paso del tiempo, ya que la edad aumenta cada año.

3. **La cantidad de dinero en una cuenta bancaria.**  
   **Es una Variable.** Porque puede cambiar con depósitos, retiros o transacciones.

4. **La velocidad de la luz en el vacío, 299,792,458 m/s.**  
   **Es una constante.** Porque es un valor fijo en la física y no varía.

5. **El radio de un círculo.**  
   **Es una variable.** Porque depende del tamaño del círculo, por lo que puede cambiar.

---

# Características de los Algoritmos. 

1. **Para elegir la ruta más corta entre varias ciudades, el algoritmo examina rutas candidatas, deteniéndose cuando los cambios en la distancia parecen lo suficientemente pequeños.**  
   **No cumple completamente con las características de un algoritmo.** Aunque describe un proceso de optimización, la condición de parada no es del todo precisa, lo que podría generar una indeterminacion y falta de determinismo.

2. **Suma los números ingresados y muestra el resultado.**  
   **No cumple completamente con las características de un algoritmo.** No especifica cuántos números se deben ingresar ni cómo se detiene la entrada, lo que genera falta de claridad en su ejecución.

3. **Un conjunto de pasos para calcular el área de un rectángulo dado su base y altura.**  
   **Sí cumple con las características de un algoritmo.** Es un procedimiento bien definido, con pasos claros y un resultado concreto (el área del rectángulo).

4. **El algoritmo cuenta el número de votos obtenidos por cada uno de los candidatos de una elección para presidente. Empieza solicitando el nombre del candidato y finaliza cuando se ingresa el valor -1.**  
   **Sí cumple con las características de un algoritmo.** Tiene una secuencia clara de pasos, entrada definida (nombre del candidato), una condición de terminación específica (-1) y un resultado bien determinado (número de votos por candidato).

---

# Comprensión de Herramientas. 

1. **El pseudocódigo utiliza símbolos estándar para representar las operaciones lógicas.**  
   **Falso.** El pseudocódigo usa una descripción textual de los pasos de un algoritmo, sin necesidad de símbolos gráficos estandarizados.

2. **Los diagramas de flujo son una representación gráfica de un algoritmo.**  
   **Cierto.** Representan visualmente los pasos de un algoritmo mediante símbolos y flechas que indican el flujo de ejecución.

3. **El pseudocódigo debe estar escrito en un lenguaje de programación específico.**  
   **Falso.** El pseudocódigo es un lenguaje informal que no sigue la sintaxis de un lenguaje de programación específico, sino que busca ser comprensible para humanos.

4. **Un diagrama de flujo siempre debe tener un inicio y un fin claramente definidos.**  
   **Cierto.** Todo diagrama de flujo debe incluir un punto de inicio y uno de fin para indicar el proceso completo del algoritmo.

---

# Estructuras de control.

Las estructuras de control son fundamentales en la programación, ya que permiten definir el flujo de ejecución de un algoritmo. Sirven para tomar decisiones, repetir acciones o seleccionar entre diferentes caminos según condiciones específicas. Estas estructuras incluyen condicionales (if-else), bucles (for, while) y estructuras de selección (switch).

### Ejemplo de la vida cotidiana
**Decidir qué ropa usar según el clima**
```Inicio
pseudocodigo
Si (la temperatura es menor a 15°C) entonces
    Usar abrigo y bufanda
Si no
    Usar ropa ligera
Fin.
```
**Explicación:** Aquí, la decisión se basa en una condición (temperatura). Si hace frío, se usa ropa abrigadora; de lo contrario, se elige ropa más ligera.

### Ejemplo con cálculos matemáticos
**Determinar si un estudiante aprueba una materia**
```Inicio
pseudocodigo
Si (promedio >= 60) entonces
    Mostrar "Aprobado"
Si no
    Mostrar "Reprobado"
Fin.
```
**Explicación:** Se usa una estructura condicional para evaluar el promedio del estudiante. Si es 60 o más, aprueba; en caso contrario, reprueba.
