# 📘 Algoritmos y su Rol en la Computación

## Basado en:
- **Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2022).** *Introduction to Algorithms* (4th Edition), MIT Press.
- **Brassard, G., & Bratley, P. (2006).** *Fundamentals of Algorithmics*.

---

## 🔢 1. The Role of Algorithms in Computing (Cormen et al., 2022)

Los algoritmos son fundamentales en la computación porque definen procesos computacionales precisos. En esencia, **un algoritmo es una secuencia bien definida de pasos computacionales que transforman una entrada en una salida**.

### 📌 1.1 ¿Qué es un Algoritmo?

Un algoritmo debe cumplir las siguientes propiedades:

- **Input:** Uno o más datos de entrada.
- **Output:** Uno o más resultados.
- **Definiteness:** Cada paso debe estar claramente definido.
- **Finiteness:** Debe completarse en un número finito de pasos.
- **Effectiveness:** Cada operación debe ser realizable con precisión y en tiempo razonable.

#### 🧠 Ejemplos comunes de algoritmos:
- Algoritmos de ordenamiento: *Merge Sort*, *Quick Sort*
- Algoritmos de búsqueda: *Búsqueda binaria*
- Algoritmos de caminos mínimos: *Dijkstra*
- Algoritmos criptográficos: *RSA*, *AES*

---

### ⚙️ 1.2 Algoritmos como Tecnología

Los algoritmos son una **tecnología abstracta** esencial que permite resolver problemas computacionales de forma eficiente.

#### ✅ Ventajas como tecnología:
- **Escalabilidad:** Funcionan con grandes volúmenes de datos.
- **Eficiencia:** Mejoran el rendimiento del software.
- **Universalidad:** Aplicables en áreas como IA, redes, gráficos, bioinformática, etc.
- **Evaluación científica:** Usan métricas formales como complejidad temporal y espacial.

> 📌 Ejemplo: Un algoritmo O(n log n) es preferible sobre uno O(n²), incluso si el segundo se ejecuta en hardware más rápido.

---

## 📖 Capítulo 1: Preliminares (Brassard & Bratley, 2006)

Este capítulo establece los fundamentos conceptuales y matemáticos del diseño de algoritmos.

### 🔍 ¿Qué es un algoritmo?

Un algoritmo es una secuencia de pasos que transforma una entrada en una salida deseada. Sirve como solución a un problema computacional.

### 🧩 Tipos de problemas:
- **Computacionales:** Ej. suma, ordenamiento.
- **De decisión:** Ej. ¿es primo un número?
- **De optimización:** Ej. camino más corto.
- **De enumeración:** Ej. generar todas las permutaciones.

---

### 🏗️ Propiedades adicionales:
- **Corrección:** Genera salidas correctas para todas las entradas válidas.
- **Eficiencia:** Usa recursos (tiempo/memoria) de forma óptima.
- **Claridad:** Fácil de entender, implementar y mantener.

---

### 🖥️ Modelos de Computación

Los algoritmos se diseñan sobre modelos abstractos como:

- **Máquina de Turing**
- **Modelo RAM (Random Access Machine)**

> En el modelo RAM, se asume que operaciones básicas como suma, acceso a memoria o comparación toman un solo paso.

---

### ⏱️ Complejidad de un Algoritmo

Permite comparar algoritmos con base en su consumo de recursos según el tamaño de la entrada `n`.

#### Notaciones comunes:

| Notación     | Nombre               | Ejemplo clásico         |
|--------------|----------------------|--------------------------|
| O(1)         | Constante            | Acceso a arreglo         |
| O(log n)     | Logarítmica          | Búsqueda binaria         |
| O(n)         | Lineal               | Recorrido de lista       |
| O(n log n)   | Lineal-logarítmica   | Merge Sort               |
| O(n²)        | Cuadrática           | Bubble Sort              |
| O(2ⁿ)        | Exponencial          | Mochila, Sudoku          |
| O(n!)        | Factorial            | Problema del viajante    |

---

## 🧠 Conclusión

Los algoritmos son el **corazón de la ciencia computacional**. Su correcto diseño, análisis y aplicación permiten resolver problemas reales de manera eficiente, independientemente del hardware o lenguaje de programación.

> 💡 Mientras el hardware mejora con el tiempo, **un buen algoritmo supera cualquier limitación tecnológica.**
