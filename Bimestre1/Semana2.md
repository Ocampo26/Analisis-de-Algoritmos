# 🧠 Capítulo 2: Comenzando con los Algoritmos

## 📚 Basado en:
- **Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2022).** *Introduction to Algorithms*, 4ta edición – Capítulo 2: Getting Started.
- **Brassard, G., & Bratley, P. (2006).** *Fundamentals of Algorithmics* – Capítulo 2: Algoritmia Elemental.

---

## ⚙️ 2.1 Insertion Sort (Cormen et al.)

### 📝 Descripción del algoritmo

**Insertion Sort** (ordenamiento por inserción) es un algoritmo simple y eficiente para listas pequeñas. Funciona como ordenar cartas en la mano: se va insertando cada elemento en la posición correcta.

```java
for j = 2 to A.length
    key = A[j]
    i = j - 1
    while i > 0 and A[i] > key
        A[i + 1] = A[i]
        i = i - 1
    A[i + 1] = key
```

## Características
    In situ: no requiere memoria adicional.
    Estable: mantiene el orden relativo de elementos con claves iguales.
    Funciona bien con listas pequeñas o casi ordenadas.
## Complejidad temporal
Caso	Comparaciones	Tiempo
Mejor caso	O(n)	Lista ya ordenada
Peor caso	O(n²)	Lista en orden inverso
Caso promedio	O(n²)	Entrada aleatoria
## Complejidad espacial

    O(1): uso constante de memoria.
📐 2.2 Analyzing Algorithms (Cormen et al.)
📋 ¿Qué significa analizar un algoritmo?

El análisis de algoritmos implica estimar:

    Tiempo de ejecución
    Espacio requerido

Utilizando un modelo como el RAM (Random Access Machine), se mide cuántas veces se ejecutan las operaciones básicas.

## Tipos de análisis

    Peor caso (worst-case): El algoritmo nunca será más lento que este caso.
    Caso promedio (average-case): Basado en entradas aleatorias.
    Mejor caso (best-case): El tiempo más rápido posible (poco útil para garantía de rendimiento).

## Notación asintótica

Se utiliza para describir el comportamiento del tiempo de ejecución cuando el tamaño de la entrada n crece:
Notación	Significado
O(g(n))	Límite superior (como máximo)
Ω(g(n))	Límite inferior (como mínimo)
Θ(g(n))	Límite ajustado (exacto)
📘 Capítulo 2: Algoritmia Elemental (Brassard & Bratley)

Brassard y Bratley abordan los algoritmos desde un enfoque pedagógico, con énfasis en las técnicas elementales.
## Enfoque del capítulo

Se presentan herramientas básicas como:

    Algoritmos iterativos y recursivos
    Ordenamiento por selección y por inserción
    Búsqueda lineal y binaria
    Representación en diagramas de flujo
    Cálculo del número de operaciones

## Ordenamiento por inserción

Similar a lo presentado por Cormen:

    Algoritmo simple y comprensible.
    Funciona bien para datos casi ordenados.
    Se compara con otros como Selection Sort, resaltando eficiencia en distintas condiciones.

## Análisis elemental

Brassard enseña a:

    Contar cuántas veces se ejecuta cada línea.
    Usar sumas aritméticas para calcular el número total de operaciones.
    Usar expresiones como n(n-1)/2 para analizar loops anidados.

 ## Conclusiones clave

    Insertion Sort es ideal como introducción al diseño y análisis de algoritmos.
    Comprender la complejidad asintótica permite tomar decisiones informadas al comparar algoritmos.
    El análisis del peor caso es la métrica más útil para garantizar rendimiento.
    Brassard enfatiza visualización y conteo exacto de operaciones, complementando el enfoque de Cormen.
