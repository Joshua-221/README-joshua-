# Fundamentos de Álgebra - Práctica 1 (Formato ASCII)

## Información del Estudiante

- **Nombre:** Joshua Cruz
- **Grupo:** 1C  
- **Carrera:** TSW  
- **Cuatrimestre:** Primero  
- **Profesor:** Jorge Javier Pedrozo Romero  

---
# Práctica: Resolución de Sistemas de Ecuaciones por Métodos de Álgebra Lineal

Este documento contiene el desarrollo completo del ejercicio donde se resuelve un sistema de ecuaciones utilizando **Gauss**, **Gauss-Jordan** y **Matriz Inversa**, incluyendo todos los procedimientos paso a paso y resultados finales.

---

# 📌 Ejercicio 1: Resolver el sistema con todos los métodos

Sistema a resolver:

$$
\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
$$

Matriz de coeficientes:

$$
A=
\begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{bmatrix}
$$

Matriz de términos independientes:

$$
B=
\begin{bmatrix}
6 \\
3 \\
2
\end{bmatrix}
$$

---

# ✨ Método 1: Eliminación de Gauss

### 🔹 Matriz aumentada inicial

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}
\right]
$$

### 🔹 Operaciones por filas  
R2 → R2 − 2R1  
R3 → R3 − R1

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

Normalizamos R2:  
R2 → (-1/3)R2

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & 1/3 & 3 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

R3 → R3 − R2

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & 1/3 & 3 \\
0 & 0 & -7/3 & -7
\end{array}
\right]
$$

### 🔹 Sustitución hacia atrás

De la última ecuación:

\[
-\frac{7}{3}z = -7 \Rightarrow z = 3
\]

De la segunda ecuación:

\[
y + \frac{1}{3}(3) = 3 \Rightarrow y = 2
\]

De la primera:

\[
x + 2 + 3 = 6 \Rightarrow x = 1
\]

### ✔ **Solución por Gauss:**
**x = 1, y = 2, z = 3**

---

# ✨ Método 2: Gauss-Jordan

Matriz aumentada inicial:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}
\right]
$$

R2 → R2 − 2R1  
R3 → R3 − R1

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

Normalización de R2:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & 1/3 & 3 \\
0 & 1 & -2 & -4
\end{array}
\right]
$$

R1 → R1 − R2  
R3 → R3 − R2

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 2/3 & 3 \\
0 & 1 & 1/3 & 3 \\
0 & 0 & -7/3 & -7
\end{array}
\right]
$$

Normalizamos R3:  
R3 → (-3/7)R3

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 2/3 & 3 \\
0 & 1 & 1/3 & 3 \\
0 & 0 & 1 & 3
\end{array}
\right]
$$

Eliminamos arriba:

R1 → R1 − (2/3)R3  
R2 → R2 − (1/3)R3  

$$
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & 1 \\
0 & 1 & 0 & 2 \\
0 & 0 & 1 & 3
\end{array}
\right]
$$

### ✔ **Solución por Gauss-Jordan:**
**x = 1, y = 2, z = 3**

---

# ✨ Método 3: Matriz Inversa

## 🧮 1. Sistema y matriz A

Sistema:

$$
\begin{cases}
x + y + z = 6 \\
2x - y + z = 3 \\
x + 2y - z = 2
\end{cases}
$$

Matriz A:

$$
A = 
\begin{bmatrix}
1 & 1 & 1 \\
2 & -1 & 1 \\
1 & 2 & -1
\end{bmatrix}
$$

---

## 🧮 2. Matriz aumentada [A | I]

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 1 & 1 & 0 & 0 \\
2 & -1 & 1 & 0 & 1 & 0 \\
1 & 2 & -1 & 0 & 0 & 1
\end{array}
\right]
$$

Se realizan operaciones hasta obtener:

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & -1/7 & 3/7 & 2/7 \\
0 & 1 & 0 & 3/7 & -2/7 & 1/7 \\
0 & 0 & 1 & 5/7 & -1/7 & -3/7
\end{array}
\right]
$$

La parte derecha es \(A^{-1}\):

### ✔ Matriz inversa encontrada:

$$
A^{-1} =
\frac{1}{7}
\begin{bmatrix}
-1 & 3 & 2 \\
3 & -2 & 1 \\
5 & -1 & -3
\end{bmatrix}
$$

---

## 🧮 3. Cálculo de la solución

Aplicamos:

\[
X = A^{-1}B
\]

Da como resultado:

x = 1
y = 2
z = 3

---

---
# Licencia

Proyecto académico bajo licencia **MIT**.
