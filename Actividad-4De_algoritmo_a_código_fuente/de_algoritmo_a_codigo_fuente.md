> - ¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en Python?

yo creo que es util para muchas cosas, entre ellas.
- La organizacion del problema
- calidad y estructura
- Disminuir la probabilidad de errores
- Ahorrar tiempo
- Facilita la cominicacion del problema

El pseudocódigo es unan herramienta esencial para diseñar y estructurar programas antes de traducirlo a python y tambien para otros lenguejes.
 
 ---

> - ¿Cuál es la diferencia entre usar int(input()) y float(input()) en Python? Si no lo tienes claro, investiga y discute lo que encontraste con el profe.


En Python, la función `input()` recibe datos del usuario en forma de cadena de texto (`str`). Para convertir estos datos a números, se pueden utilizar `int()` o `float()`, dependiendo del tipo de número que se necesite.

### `int(input())`
- Convierte la entrada del usuario a un número entero (`int`).
- No admite valores decimales; si el usuario ingresa un número con decimales, se generará un error.
- Ejemplo:
  ```python
  numero = int(input("Ingrese un número entero: "))
  print(f"El número ingresado es: {numero}")
  ```

### `float(input())`
- Convierte la entrada del usuario a un número de punto flotante (`float`).
- Admite tanto números enteros como decimales.
- Ejemplo:
  ```python
  numero = float(input("Ingrese un número decimal: "))
  print(f"El número ingresado es: {numero}")
  ```

### Diferencias clave
| Característica  | `int(input())` | `float(input())` |
|---------------|---------------|---------------|
| Acepta enteros | ✅ | ✅ |
| Acepta decimales | ❌ | ✅ |
| Redondeo automático | No aplica | No aplica |
| Tipo de dato resultante | `int` | `float` |

Fuente: [Documentación oficial de Python](https://docs.python.org/3/library/functions.html#input)



> - Escribe tu propio pseudocódigo para calcular el promedio de una lista de calificaciones y tradúcelo a Python.

### Pseudocódigo para calcular el promedio de una lista de calificaciones

INICIO  
    Definir lista de calificaciones  
    Calcular la suma de todas las calificaciones  
    Contar la cantidad de calificaciones  
    Si la cantidad es mayor que 0
     entonces  
        Calcular el promedio (suma / cantidad)  
        Mostrar el promedio  
    Si no  
        Mostrar mensaje "No hay calificaciones para promediar"  
FIN  

---

### Código en Python

```python
def calcular_promedio(calificaciones):
    if len(calificaciones) == 0:
        return "No hay calificaciones para promediar"
    
    suma = sum(calificaciones)
    cantidad = len(calificaciones)
    promedio = suma / cantidad
    return promedio

# Ejemplo de uso
calificaciones = [85, 90, 78, 92, 88]
resultado = calcular_promedio(calificaciones)
print("El promedio es:", resultado)
