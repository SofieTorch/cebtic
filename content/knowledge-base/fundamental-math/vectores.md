---
title: Vectores
type: docs
prev: /
next: fundamental-math/matrices
---

| Tags           | Autor                          | Estado      |
| -------------- | ------------------------------ | ----------- |
| Álgebra lineal | Luis Eduardo Acebey Villarroel | En progreso |

Algoritmos de Machine Learning: Regresión lineal (https://www.notion.so/Regresi-n-lineal-5bc459048d474296998d4d9cbadb9ecf?pvs=21), Regresión logistica (https://www.notion.so/Regresi-n-logistica-119a8b553e1841ea925a3435ec52127b?pvs=21)

## Propiedades Fundamentales de los Vectores

### 1. Magnitud (Norma):

- La magnitud de un vector es una medida de su longitud o tamaño. Para un vector $v=(v1​,v2​,...,vn​)$, la magnitud se calcula como:
  $$ \|\mathbf{v}\| = \sqrt{v_1^2 + v_2^2 + \cdots + v_n^2} $$
- **Interpretación matemática:** Representa la distancia desde el origen hasta el punto definido por el vector en un espacio euclidiano.
- **Relevancia en machine learning:** La magnitud de un vector puede ser usada en algoritmos de normalización para escalar características de datos y mejorar la convergencia de los modelos de aprendizaje.

![Untitled](Vectores%2054528ad840b645bc9d4e9c87c4f23ecb/Untitled.png)

### 2. Dirección:

- La dirección de un vector indica hacia dónde apunta en el espacio. Se puede obtener dividiendo el vector por su magnitud, obteniendo un vector unitario.

  $$\hat{\mathbf{v}} = \frac{\mathbf{v}}{\|\mathbf{v}\|}$$

- **Interpretación matemática:** Define la orientación del vector sin considerar su longitud.
- **Relevancia en machine learning:** Es importante para entender la dirección de los gradientes en algoritmos de optimización como el descenso de gradiente.

![Untitled](Vectores%2054528ad840b645bc9d4e9c87c4f23ecb/Untitled%201.png)

### 3. Suma de Vectores:

- La suma de dos vectores u y v se realiza componente a componente:

  $$\mathbf{u} + \mathbf{v} = (u_1 + v_1, u_2 + v_2, \ldots, u_n + v_n)$$

- **Interpretación matemática:** La suma de vectores resulta en un nuevo vector que puede interpretarse como la combinación de los desplazamientos representados por cada vector.
- **Relevancia en machine learning:** Es fundamental en el cálculo de las actualizaciones de parámetros y la combinación de múltiples efectos en modelos de ensamble.

### 4. Producto Escalar (Producto Punto):

- El producto escalar de dos vectores u y v es un número (escalar) calculado como:

  $$\mathbf{u} \cdot \mathbf{v} = u_1 v_1 + u_2 v_2 + \cdots + u_n v_n$$

- **Interpretación matemática:** Representa la proyección de un vector sobre otro y puede indicar el ángulo entre ellos.
- **Relevancia en machine learning:** Se usa en medidas de similitud, como el coseno de la similitud, y en funciones de activación de redes neuronales.

### 5. Producto Vectorial:

- El producto vectorial es aplicable en el espacio tridimensional y resulta en un nuevo vector perpendicular a los vectores originales u y v:

  $$\mathbf{u} \times \mathbf{v} = \begin{vmatrix}\mathbf{i} & \mathbf{j} & \mathbf{k} \\u_1 & u_2 & u_3 \\v_1 & v_2 & v_3 \\\end{vmatrix} = (u_2 v_3 - u_3 v_2, u_3 v_1 - u_1 v_3, u_1 v_2 - u_2 v_1)$$

- **Interpretación matemática:** Representa el área del paralelogramo formado por los dos vectores y su orientación.
- **Relevancia en machine learning:** Aunque menos común, es útil en problemas de geometría computacional y en cálculos de determinantes y matrices de rotación.

## Propiedades extra

![Untitled](Vectores%2054528ad840b645bc9d4e9c87c4f23ecb/Untitled%202.png)
