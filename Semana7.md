# 📘 Tema 3: Notación Asintótica  
**Fuente:** Brassard & Bratley (2006) – *Fundamentos de Algoritmia*

---

## 🎯 Objetivo

Proporcionar una base matemática para expresar la complejidad temporal o espacial de los algoritmos, permitiendo comparar su eficiencia y comportamiento a medida que el tamaño de la entrada crece.

---

## ⚖️ Conceptos Clave

Cuando analizamos algoritmos, el crecimiento de su tiempo de ejecución o uso de recursos se describe mediante funciones matemáticas en función de la variable **n** (tamaño de la entrada).

Para comparar funciones f(n) y g(n):

- **f(n) crece más lento que g(n)** si:  
  \> Lim(n→∞) f(n)/g(n) = 0

- **f(n) y g(n) crecen al mismo ritmo** si:  
  \> Lim(n→∞) f(n)/g(n) = c (constante distinta de cero)

- **f(n) crece más rápido que g(n)** si:  
  \> Lim(n→∞) f(n)/g(n) = ∞

---

## 📌 Notaciones Asintóticas Fundamentales

### 1. Notación **O** (Big O) — Cota Superior

Describe el comportamiento en el peor caso.  
Existe c > 0 y n₀ tal que para todo n ≥ n₀:

$$
T(n) \leq c \cdot f(n)
$$

Significa que T(n) crece **a lo más** tan rápido como f(n).

---

### 2. Notación **Ω** (Omega) — Cota Inferior

Describe el comportamiento en el mejor caso.  
Existe c > 0 y n₀ tal que para todo n ≥ n₀:

$$
T(n) \geq c \cdot f(n)
$$

Significa que T(n) crece **al menos** tan rápido como f(n).

---

### 3. Notación **Θ** (Theta) — Cota Ajustada

Describe un crecimiento exacto, acotado tanto por arriba como por abajo.  
Existen c₁, c₂ > 0 y n₀ tal que para todo n ≥ n₀:

$$
c_1 \cdot f(n) \leq T(n) \leq c_2 \cdot f(n)
$$

Esto indica que T(n) y f(n) tienen el **mismo orden de crecimiento**.

---

## 🧠 Reglas y Ejemplos útiles

- O(n + log n) = O(n)  
- O(n² + n) = O(n²)  
- O(c · f(n)) = O(f(n)) para cualquier constante c > 0  

---

## 🧪 Ejemplos de crecimiento asintótico

| Función de tiempo        | Clasificación asintótica |
|-------------------------|-------------------------|
| 5n + 7                  | O(n)                    |
| n log n + 3n            | O(n log n)              |
| 3n² + 2n + 1            | O(n²)                   |
| 2ⁿ                      | O(2ⁿ)                   |

---

## 📊 Tabla de Clases de Complejidad Comunes

| Clase        | Ejemplo                       | Tiempo Típico         |
|--------------|------------------------------|----------------------|
| O(1)         | Acceso a arreglo              | Constante            |
| O(log n)     | Búsqueda binaria             | Logarítmico          |
| O(n)         | Búsqueda lineal              | Lineal               |
| O(n log n)   | Merge Sort, Quick Sort       | Linealítmico         |
| O(n²)        | Insertion Sort, Selection Sort | Cuadrático          |
| O(2ⁿ)        | Fuerza bruta en problemas NP | Exponencial          |

---

## 🧠 Reflexión Final

- Las notaciones asintóticas permiten abstraerse del hardware y enfocarse en la eficiencia algorítmica.  
- Son esenciales para diseñar y comparar algoritmos.  
- El análisis se basa en el comportamiento para entradas grandes (n → ∞).  
