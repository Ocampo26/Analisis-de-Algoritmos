# 📘 Semana 14 – Algoritmos Probabilistas

## 📖 Fuente:
**Brassard, G. & Bratley, P. (2000).** *Fundamentos de Algoritmia*. Tema 10: Algoritmos Probabilistas.

---

## 🎯 ¿Qué es un algoritmo probabilista?

Es un algoritmo que toma decisiones en base a valores aleatorios. Utiliza un generador de números pseudoaleatorios para guiar parte o toda su ejecución.

### ✅ Propósito:
- Mejorar el **rendimiento promedio**.
- Resolver problemas donde los algoritmos deterministas son demasiado lentos o complejos.
- Afrontar incertidumbre o variabilidad en los datos.

---

## 🧠 Clasificación de algoritmos probabilistas

### 1. **Algoritmos Monte Carlo**
- **Siempre rápidos**, pero **pueden fallar** con una baja probabilidad.
- **Ejemplo**: Verificar si un número es primo con error aceptable.

### 2. **Algoritmos Las Vegas**
- **Siempre correctos**, pero el **tiempo de ejecución es aleatorio**.
- **Ejemplo**: QuickSort con pivote aleatorio.

---

## 🔢 Generación de números aleatorios

- Utilizan **generadores congruenciales lineales (LCG)**:
  
  `Xₙ₊₁ = (a * Xₙ + c) mod m`

- Necesarios para alimentar de aleatoriedad al algoritmo.

---

## 📌 Ejemplos discutidos en el capítulo

### 🧪 Pruebas de primalidad probabilistas:
- Ej: Algoritmo de **Miller-Rabin** (Monte Carlo).
- Más rápidos que métodos deterministas, aunque con ligera probabilidad de error.

### 🎲 Selección aleatoria:
- Selección de un elemento aleatorio con distribución uniforme.
- Uso en juegos, simulaciones, y sistemas adaptativos.

---

## 📊 Evaluación de rendimiento

| Algoritmo     | Correctitud | Tiempo de ejecución |
|---------------|-------------|----------------------|
| Determinista  | Siempre     | Determinístico       |
| Monte Carlo   | Probable    | Determinístico       |
| Las Vegas     | Siempre     | Probabilístico       |

---

## 🔍 Ventajas de los algoritmos probabilistas

- En muchos casos, son **más rápidos** que los deterministas.
- Útiles cuando el espacio de búsqueda es demasiado grande.
- Buena aproximación cuando no se necesita una respuesta exacta.

---

## ⚠️ Consideraciones

- Importancia de tener un **buen generador aleatorio**.
- Evaluar la **probabilidad de error**.
- A veces, se pueden repetir varias veces para reducir el error.

---

## 📚 Referencia

Brassard, G., & Bratley, P. (2000). *Fundamentos de algoritmia* (Cap. 10). Pearson Educación.
----------------------------------------------------
![Imagen de WhatsApp 2025-07-27 a las 22 41 30_bbd348eb](https://github.com/user-attachments/assets/d89eb71d-07f4-45d3-9752-fd0aa05f4765)
![Imagen de WhatsApp 2025-07-27 a las 22 41 40_0b3e4bd3](https://github.com/user-attachments/assets/4bcbffc5-1e2c-4350-bb9e-74a1c300c7e3)
![Imagen de WhatsApp 2025-07-27 a las 22 41 50_46672961](https://github.com/user-attachments/assets/ce1049b2-f299-47e6-938b-d01b09e2ed29)
![Imagen de WhatsApp 2025-07-27 a las 22 42 05_9e88b8cd](https://github.com/user-attachments/assets/281d4549-66fb-46f5-aba6-b4e1b8291302)
![Imagen de WhatsApp 2025-07-27 a las 22 42 16_f4256e85](https://github.com/user-attachments/assets/c8aa01c2-1d5e-4699-ba42-1a0d11fe4198)
![Imagen de WhatsApp 2025-07-27 a las 22 42 30_8a67b846](https://github.com/user-attachments/assets/c51d1e0a-8109-40b8-bfd1-8530c6884657)


