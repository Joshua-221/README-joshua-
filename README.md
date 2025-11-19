# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Joshua Isaí Cruz Mosqueda
## Actividad #18. Matrices: Determinantes y operaciones básicas
___
#Objetivo 

Realizar ejercicios prácticos sobre el cálculo de determinantes de matrices de distintos tamaños (2x2, 3x3 y 4x4) usando varios métodos, además de comprobar sus propiedades y sus aplicaciones geométricas.
___

## Índice
- [Ejercicio 1: Determinantes 2x2](#ejercicio-1-determinantes-2x2)
- [Ejercicio 2: Regla de Sarrus](#ejercicio-2-regla-de-sarrus)
- [Ejercicio 3: Método de cofactores](#ejercicio-3-método-de-cofactores)
- [Ejercicio 4: Verificar propiedades](#ejercicio-4-verificar-propiedades)
- [Ejercicio 5: Aplicación geométrica](#ejercicio-5-aplicación-geométrica)
---

## Ejercicio 1: Determinantes 2x2

### Objetivo
Calcular el determinante de matrices 2x2 usando la fórmula correspondiente y aplicar este resultado en ejercicios básicos.

---

Calcula el determinante de las siguientes matrices 2x2:

$$A = \begin{pmatrix}
5 & 2 \\
3 & 1  
\end{pmatrix}, \quad 
B = \begin{pmatrix}
-1 & 4 \\
2 & -8
\end{pmatrix}$$

$$C = \begin{pmatrix}
6 & 9 \\
2 & 3
\end{pmatrix}, \quad 
D = \begin{pmatrix}
0 & 5 \\
-5 & 0
\end{pmatrix}$$

### Solución

**Paso 1:** Para una matriz 2x2, el determinante se obtiene con:
$$\det(A) = ad - bc$$

**Paso 2:** Determinantes de cada matriz:

- **A:**  
  $$\det(A) = (5)(1) - (2)(3) = -1$$

- **B:**  
  $$\det(B) = (-1)(-8) - (4)(2) = 0$$

- **C:**  
  $$\det(C) = (6)(3) - (9)(2) = 0$$

- **D:**  
  $$\det(D) = (0)(0) - (5)(-5) = 25$$
---

# Ejercicio 2: Operaciones con matrices

## Objetivo del ejercicio:

Realizar operaciones aritméticas básicas con matrices, incluyendo suma, resta, multiplicación y transposición.

Dadas las matrices:

$$ A = \begin{bmatrix}
2 & -1 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
5 & 2 \\
-1 & 3 
\end{bmatrix} $$

Calcula: 

### a) Suma de matrices: \( A + B \)
$$ A + B = \begin{bmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3
\end{bmatrix} = \begin{bmatrix}
7 & 1 \\
2 & 7
\end{bmatrix} $$

### b) Resta  y  multiplicación de matrices: \(2A - B \)

$$ 2A - B = 2 \begin{bmatrix}
2 & -1 \\
3 & 4
\end{bmatrix} - \begin{bmatrix}
5 & 2 \\    
-1 & 3
\end{bmatrix} = \begin{bmatrix}
4 & -2 \\
6 & 8
\end{bmatrix} - \begin{bmatrix}
5 & 2 \\
-1 & 3
\end{bmatrix} = \begin{bmatrix}
-1 & -4 \\
7 & 5
\end{bmatrix} $$

### c) Multiplicación de matrices: \( AB \)
$$ AB = \begin{bmatrix}
2 & -1 \\
3 & 4
\end{bmatrix} \begin{bmatrix}
5 & 2 \\
-1 & 3
\end{bmatrix} = \begin{bmatrix}
2\cdot5+(-1)\cdot(-1) & 2\cdot2+(-1)\cdot3\\
3\cdot5+4\cdot(-1)    & 3\cdot2+4\cdot3
\end{bmatrix} = \begin{bmatrix}
11 & 1 \\
11 & 18
\end{bmatrix} $$

### d) Multiplicación de matrices: \( BA \)
$$ BA = \begin{bmatrix}
5 & 2 \\
-1 & 3
\end{bmatrix} \begin{bmatrix}
2 & -1 \\
3 & 4
\end{bmatrix} = \begin{bmatrix}
(5\cdot2) + (2\cdot3) & (5\cdot-1) + (2\cdot4) \\
(-1\cdot2) + (3\cdot3) & (-1\cdot-1) + (3\cdot4)
\end{bmatrix} = \begin{bmatrix}
16 & 3 \\
7 & 13
\end{bmatrix} $$

### e) Transpuesta de la matriz A: \( A^T \)
$$ A^T = \begin{bmatrix}
2 & 3 \\
-1 & 4
\end{bmatrix} $$

---

# Ejercicio 3: Multiplicación cadena

## Objetivo del ejercicio:
Verificar la propiedad asociativa de la multiplicación de matrices mediante el cálculo de productos en cadena.

---

Verificar que $(AB)C = A(BC)$ 

Dadas las matrices:

$$ A = \begin{bmatrix}
1 & 2 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
2 & 0 \\
1 & 3 
\end{bmatrix}, \quad C = \begin{bmatrix}
1 & 1 \\
0 & 2
\end{bmatrix} $$

### a) Calcular \( (AB)C \)
$$ AB = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix} \begin{bmatrix}
2 & 0 \\
1 & 3
\end{bmatrix} = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot0) + (2\cdot3) \\
(3\cdot2) + (4\cdot1) & (3\cdot0) + (4\cdot3)
\end{bmatrix} = \begin{bmatrix}
4 & 6 \\
10 & 12
\end{bmatrix} $$
$$ (AB)C = \begin{bmatrix}
4 & 6 \\
10 & 12
\end{bmatrix} \begin{bmatrix}
1 & 1 \\
0 & 2
\end{bmatrix} = \begin{bmatrix}
(4\cdot1) + (6\cdot0) & (4\cdot1) + (6\cdot2) \\
(10\cdot1) + (12\cdot0) & (10\cdot1) + (12\cdot2)
\end{bmatrix} = \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

### b) Calcular \( A(BC) \)
$$ BC = \begin{bmatrix}
2 & 0 \\
1 & 3
\end{bmatrix} \begin{bmatrix}
1 & 1 \\
0 & 2
\end{bmatrix} = \begin{bmatrix}
(2\cdot1) + (0\cdot0) & (2\cdot1) + (0\cdot2) \\
(1\cdot1) + (3\cdot0) & (1\cdot1) + (3\cdot2)
\end{bmatrix} = \begin{bmatrix}
2 & 2 \\
1 & 7
\end{bmatrix} $$
$$ A(BC) = \begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix} \begin{bmatrix}
2 & 2 \\
1 & 7
\end{bmatrix} = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot2) + (2\cdot7) \\
(3\cdot2) + (4\cdot1) & (3\cdot2) + (4\cdot7)
\end{bmatrix} = \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

Conclusión: Por lo que se verificará que $(AB)C = A(BC)$.



