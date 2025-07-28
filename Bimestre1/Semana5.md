# 📘 Capítulo 3: Notación Asintótica
**Fundamentals of Algorithmics – Brassard & Bratley (2006)**

---

## 🎯 Objetivo del Capítulo

Brindar una base matemática sólida para analizar y comparar algoritmos, utilizando herramientas que describan su eficiencia en función del tamaño de la entrada (n).

---

## ⚖️ Comparación de funciones de crecimiento

Dadas dos funciones f(n) y g(n):

- f(n) crece más lentamente que g(n) si:  
  f(n) / g(n) → 0 cuando n → ∞

- f(n) y g(n) crecen al mismo ritmo si:  
  f(n) / g(n) → constante ≠ 0 cuando n → ∞

- f(n) crece más rápidamente que g(n) si:  
  f(n) / g(n) → ∞ cuando n → ∞

---

## 📌 Notaciones Asintóticas

### 🔹 Notación O — Cota Superior (Límite Superior)

Describe el peor caso del algoritmo, el máximo tiempo o recursos requeridos.

T(n) pertenece a O(f(n)) si existen constantes c > 0 y n₀ tal que para todo n ≥ n₀:

> T(n) ≤ c * f(n)

---

### 🔸 Notación Ω — Cota Inferior (Límite Inferior)

Describe el mejor caso del algoritmo, el menor tiempo o recursos requeridos.

T(n) pertenece a Ω(f(n)) si existen constantes c > 0 y n₀ tal que para todo n ≥ n₀:

> T(n) ≥ c * f(n)

---

### ⚖️ Notación Θ — Cota Ajustada

Define una acotación exacta: el algoritmo se comporta dentro de un rango determinado de eficiencia.

T(n) pertenece a Θ(f(n)) si existen constantes c₁, c₂ > 0 y n₀ tal que para todo n ≥ n₀:

> c₁ * f(n) ≤ T(n) ≤ c₂ * f(n)

---

## 🧠 Reglas prácticas con notación O

- O(n + log n) = O(n)
- O(n² + n) = O(n²)
- O(c * f(n)) = O(f(n)) para cualquier constante c > 0

---

## 📊 Tabla de clases de complejidad

| Clase        | Ejemplo de algoritmo             | Tiempo típico    |
|--------------|----------------------------------|------------------|
| O(1)         | Acceso a un arreglo              | Constante        |
| O(log n)     | Búsqueda binaria                 | Logarítmico      |
| O(n)         | Búsqueda lineal                  | Lineal           |
| O(n log n)   | Merge Sort, Quick Sort (mejor)   | Linealítmico     |
| O(n²)        | Insertion Sort, Selection Sort   | Cuadrático       |
| O(2ⁿ)        | Fuerza bruta en problemas NP     | Exponencial      |

---

## 🧠 Reflexiones clave

- Las notaciones asintóticas son esenciales para analizar algoritmos independientemente del hardware.
- Permiten comparar diferentes soluciones y seleccionar las más eficientes.
- Brassard & Bratley usan un enfoque matemático claro para entender cómo se comportan los algoritmos en función del tamaño de la entrada.

![Semana_5](https://github.com/user-attachments/assets/9ede631b-6185-4e12-ba9a-a34e5932d558)

