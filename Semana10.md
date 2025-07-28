# 📘 6.4 Grafos: Caminos mínimos
**Fuente:** Brassard, G. & Bratley, P. (2000). *Fundamentos de Algoritmos*.

## 🎯 Objetivo

Resolver el problema de encontrar el **camino más corto** entre nodos en un **grafo ponderado**, donde cada arista tiene un costo o peso asociado.

## 🔍 Descripción del problema

- Dado un grafo \( G = (V, E) \) con pesos positivos en las aristas.
- Se busca el camino de **menor costo**:
  - Desde un **único nodo origen** a todos los demás.
  - Entre **todos los pares de nodos**.

## ⚙️ Algoritmos principales

### 1. 🧭 Algoritmo de Dijkstra

- **Tipo:** Voraz.
- **Entrada:** Grafo con pesos **no negativos**.
- **Salida:** Caminos mínimos desde un nodo origen.
- **Estrategia:**
  - Inicializa distancias con infinito, excepto el nodo origen (0).
  - Iterativamente selecciona el nodo no visitado más cercano.
  - Actualiza las distancias de sus vecinos.
- **Complejidad:**
  - Con cola de prioridad: \( O((V + E) \log V) \).
- **Restricción:** No funciona si hay pesos negativos.

### 2. 🔁 Algoritmo de Floyd-Warshall

- **Tipo:** Programación dinámica (no voraz puro).
- **Entrada:** Grafo dirigido o no dirigido, con pesos (pueden ser negativos).
- **Salida:** Caminos mínimos entre **todos los pares de nodos**.
- **Estrategia:**
  - Usa matriz de distancias.
  - Considera cada nodo como intermediario.
  - Actualiza la matriz si encuentra un camino más corto.

## 🧠 Algoritmo Voraz

- El algoritmo de Dijkstra es voraz porque:
  - Siempre elige la solución **localmente óptima** (el nodo más cercano).
  - Bajo ciertas condiciones, esta elección produce una **solución global óptima**.

## 🧪 Ejemplo (Dijkstra)

Grafo:

| Arista | Peso |
|--------|------|
| A-B    | 1    |
| A-C    | 4    |
| B-C    | 2    |
| B-D    | 5    |
| C-D    | 1    |

Camino mínimo desde **A** a **D**:
- A → B → C → D
- Costo total: 1 + 2 + 1 = **4**

## 📌 Conclusión

- El subtema aborda cómo los algoritmos voraces pueden aplicarse eficazmente a problemas de caminos mínimos.
- Dijkstra es eficiente y garantiza soluciones óptimas cuando los pesos son no negativos.
-------------------------------------------------------------------------------------------------------------
![Imagen de WhatsApp 2025-07-27 a las 22 31 24_00501fe9](https://github.com/user-attachments/assets/7262a6dc-70d0-4c08-bafe-88ebfdffd561)
![Imagen de WhatsApp 2025-07-27 a las 22 31 32_742229ea](https://github.com/user-attachments/assets/bb286f34-85f3-4d25-9787-4df4a2f74101)

