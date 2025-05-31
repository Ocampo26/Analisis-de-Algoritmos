# 📘 Capítulo 3: Notación Asintótica y Tiempos de Ejecución

## 📚 Basado en:
- **Cormen et al. (2022)** – *Introduction to Algorithms*, 4ta edición – Capítulo 3: *Characterizing Running Times*
- **Brassard & Bratley (2006)** – *Fundamentals of Algorithmics* – Capítulo 3: *Notación Asintótica*

---

## 🧠 Reglas útiles para trabajar con notaciones

- `O(n + log n) = O(n)`
- `O(n² + n) = O(n²)`
- `O(c · f(n)) = O(f(n))`, para cualquier constante `c > 0`

---

## 🧪 Ejemplos de crecimiento

| Función de tiempo        | Clasificación asintótica |
|--------------------------|--------------------------|
| `5n + 7`                 | `O(n)`                   |
| `n log n + 3n`           | `O(n log n)`             |
| `3n² + 2n + 1`           | `O(n²)`                  |
| `2ⁿ`                     | `O(2ⁿ)`                  |

---

## 📖 Parte II: Notación Asintótica (Brassard & Bratley)

### 🎯 Objetivo

Brindar una **base matemática sólida** para expresar la **complejidad algorítmica**, destacando la **eficiencia relativa** entre algoritmos.

---


---

## 📊 Tabla comparativa de clases de complejidad

| Clase        | Ejemplo de algoritmo             | Tiempo típico    |
|--------------|----------------------------------|------------------|
| `O(1)`       | Acceso a un arreglo              | Constante        |
| `O(log n)`   | Búsqueda binaria                 | Logarítmico      |
| `O(n)`       | Búsqueda lineal                  | Lineal           |
| `O(n log n)` | Merge Sort, Quick Sort (mejor)   | Linealítmico     |
| `O(n²)`      | Insertion Sort, Selection Sort   | Cuadrático       |
| `O(2ⁿ)`      | Algoritmos por fuerza bruta (NP) | Exponencial      |

---

## 🧠 Conclusiones conjuntas

- Las **notaciones asintóticas** son esenciales para **evaluar y comparar algoritmos**.
- Tanto **Cormen** como **Brassard** presentan formalismos similares pero con enfoques distintos.
- Al diseñar algoritmos, se prefiere siempre un **orden de crecimiento más bajo**, especialmente en el **peor caso**.
- Como resumen:

> “En algoritmos, lo que más importa no es el número exacto de operaciones, sino cómo este número crece con el tamaño de la entrada.” — *Brassard & Bratley*

