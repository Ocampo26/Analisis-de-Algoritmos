# 📘 Semana 15 – Algoritmos Probabilistas (Parte 2)

## 🎯 ¿Qué son los algoritmos probabilistas?

Son algoritmos que **usan números aleatorios** como parte de su lógica. A diferencia de los algoritmos deterministas, **su resultado o comportamiento puede cambiar en diferentes ejecuciones**, incluso con la misma entrada.

---

## 🧪 Tipos de algoritmos probabilistas

### 1. **Algoritmos Monte Carlo**
- **Rápidos**, pero pueden dar respuestas **incorrectas con baja probabilidad**.
- Útiles cuando se puede aceptar un pequeño margen de error.
- Ejemplo clásico: Prueba de primalidad de Miller-Rabin.

### 2. **Algoritmos Las Vegas**
- **Siempre dan una respuesta correcta**, pero su tiempo de ejecución es **probabilístico**.
- Ejemplo clásico: QuickSort con pivote aleatorio.

---

## 🧠 Conceptos clave

- **Probabilidad de error**: En Monte Carlo, se puede reducir repitiendo el algoritmo varias veces.
- **Uso de generadores de números pseudoaleatorios (PRNG)**: como base para el comportamiento aleatorio.

---

## 🧩 Ejemplo: Prueba de primalidad (Miller-Rabin)

Un algoritmo Monte Carlo para determinar si un número es primo:

1. Selecciona aleatoriamente un número "a".
2. Verifica si "a" es testigo de la composición de "n".
3. Si encuentra un testigo, dice que "n" no es primo.
4. Si no, **puede ser primo** con alta probabilidad.

---

## 🧮 Comparación

| Tipo        | ¿Correcto siempre? | ¿Tiempo fijo? | Uso de aleatoriedad |
|-------------|--------------------|---------------|----------------------|
| Determinista | ✅ Sí             | ✅ Sí        | ❌ No                |
| Monte Carlo | ❌ No (probable)   | ✅ Sí        | ✅ Sí               |
| Las Vegas   | ✅ Sí             | ❌ No        | ✅ Sí               |

---

## 💻 Aplicaciones

- Criptografía (RSA, claves públicas)
- Simulación de sistemas físicos o financieros
- Algoritmos de búsqueda y optimización
- Pruebas de primalidad
- Aprendizaje automático

---

## 📚 Referencias

- Brassard, G., & Bratley, P. (2000). *Algorithmics: Theory and Practice*.
- Cormen, T. H., et al. (2022). *Introduction to Algorithms*.

