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

## Ejercicio 2: Regla de Sarrus

### Objetivo
Calcular el determinante de matrices 3x3 usando la regla de Sarrus.

---

Determina el valor de:

$$E = \begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0
\end{pmatrix}, \quad 
F = \begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2
\end{pmatrix}$$

### Solución

**Regla de Sarrus:**  
Extender la matriz copiando sus dos primeras filas y sumar diagonales principales menos diagonales secundarias.

---

### Matriz E

**Extensión:**

$$\det(E) = \begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
\hline
1 & 2 & 3 \\
0 & 1 & 4
\end{pmatrix}$$

**Diagonales principales:**
- $1\cdot1\cdot0 = 0$
- $2\cdot4\cdot5 = 40$
- $3\cdot0\cdot6 = 0$

**Diagonales secundarias:**
- $3\cdot1\cdot5 = 15$
- $2\cdot0\cdot1 = 0$
- $1\cdot4\cdot6 = 24$

**Resultado:**
$$\det(E) = (0 + 40 + 0) - (15 + 0 + 24) = 1$$

---

### Matriz F

**Extensión:**

$$\det(F) = \begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
\hline
2 & -1 & 3 \\
1 & 4 & 0
\end{pmatrix}$$

**Diagonales principales:**
- $2\cdot4\cdot(-2) = -16$
- $(-1)\cdot0\cdot3 = 0$
- $3\cdot1\cdot2 = 6$

**Diagonales secundarias:**
- $3\cdot4\cdot3 = 36$
- $2\cdot0\cdot2 = 0$
- $(-2)\cdot1\cdot(-1) = 2$

**Resultado:**
$$\det(F) = (-16 + 0 + 6) - (36 + 0 + 2) = -48$$


---

## Ejercicio 3: Método de cofactores

### Objetivo
Calcular el determinante de una matriz 3x3 usando cofactores.

---

Determina el valor de:

$$G = \begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1   
\end{pmatrix}$$

### Solución

**Método:**  
Se elige una fila o columna, se aplican signos alternados y cada elemento se multiplica por el determinante de su menor.

---

### Expansión por la primera fila

$$
\det(G) = 
1 \cdot \begin{vmatrix}
3 & 1 \\
0 & 1
\end{vmatrix}
- 
0 \cdot \begin{vmatrix}
-1 & 1 \\
2 & 1
\end{vmatrix}
+ 
2 \cdot \begin{vmatrix}
-1 & 3 \\
2 & 0
\end{vmatrix}
$$

**Cálculo de menores:**

- $1(3\cdot1 - 1\cdot0) = 3$
- $0(\dots) = 0$
- $2(-1\cdot0 - 3\cdot2) = 2(-6) = -12$

**Resultado final:**

$$\det(G) = 3 - 12 = -9$$






