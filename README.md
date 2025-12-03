# Fundamentos de Álgebra - Práctica 1 (Formato ASCII)

## Información del Estudiante

- **Nombre:** Joshua Cruz
- **Grupo:** 1C  
- **Carrera:** TSW  
- **Cuatrimestre:** Primero  
- **Profesor:** Jorge Javier Pedrozo Romero  

---

# Descripción del Proyecto

Este repositorio contiene mi desarrollo correspondiente a la práctica de **Fundamentos de Álgebra**, implementando operaciones básicas con matrices mediante JavaScript.

La práctica incluye:

- Cálculo de determinantes  
- Suma y resta de matrices  
- Multiplicación de matrices  
- Representación en consola con formato ASCII  
- Explicación paso a paso de cada proceso  

El objetivo es comprender los fundamentos del álgebra lineal y reforzar habilidades lógicas y matemáticas.

---

# Ejercicio 1: Determinante de una matriz 2×2

Dada la matriz:
A = | a b |
| c d |


El determinante se obtiene con la fórmula:

det(A) = ad - bc

Ejemplo utilizado en esta práctica:

A = | 2 1 |
| 1 3 |

Cálculo:

det(A) = (23) - (11) = 6 - 1 = 5

---

# Ejercicio 2: Suma, Resta y Multiplicación de Matrices

Matrices dadas:

A = | 2 1 |
| 1 3 |
B = | 1 2 |
| 3 1 |


---

## ➕ Suma de matrices (A + B)

A + B = | 2+1 1+2 |
| 1+3 3+1 |
A + B = | 3 3 |
| 4 4 |


---

## ➖ Resta de matrices (A - B)

A - B = | 2-1 1-2 |
| 1-3 3-1 |
A - B = | 1 -1 |
| -2 2 |


---

## ✖ Multiplicación de matrices (AB)

Proceso:

AB = | (21 + 13) (22 + 11) |
| (11 + 33) (12 + 31) |

Resultado:

AB = | 5 5 |
| 10 5 |

---

# Ejercicio 3: Determinantes de A, B y AB

### Determinante de A

det(A) = (23) - (11) = 5

### Determinante de B

det(B) = (11) - (23) = -5

### Determinante de AB

det(AB) = (55) - (510) = 25 - 50 = -25

### Verificación de propiedad

det(AB) = det(A) * det(B)
-25 = 5 * -5

✔ Propiedad verificada correctamente.

---

# Procesos adicionales incluidos

- Validación de datos numéricos antes de operar.  
- Impresión de matrices en formato ASCII para mayor claridad.  
- Separación de cálculos en funciones individuales.  
- Explicación de cada operación paso a paso.  
- Comprensión de propiedades matemáticas fundamentales.  

---

# Licencia

Proyecto académico bajo licencia **MIT**.
