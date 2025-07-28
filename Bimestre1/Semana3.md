  # 🧠 2.3 Designing Algorithms

## 📚 Basado en:
- **Cormen, T. H., Leiserson, C. E., Rivest, R. L., & Stein, C. (2022).**
  *Introduction to Algorithms*, 4ta edición – Capítulo 2.3: Designing Algorithms

---

## 🎯 ¿Qué es diseñar un algoritmo?

Diseñar un algoritmo significa idear una **estrategia paso a paso** que solucione un problema de forma clara, eficiente y correcta. Esto involucra tanto **la lógica** como el **análisis de rendimiento**.

---

## 🧩 Elementos clave del diseño de algoritmos

### 1. **Entender el problema**
Antes de pensar en una solución, es fundamental:
- Comprender completamente el **problema** y sus **restricciones**.
- Definir claramente la **entrada** y la **salida** esperadas.
- Identificar ejemplos representativos para testear.

### 2. **Elegir una estrategia de diseño**
Existen técnicas generales para construir algoritmos:

| Técnica               | Descripción breve |
|------------------------|-------------------|
| **Dividir y vencer**   | Dividir el problema en subproblemas más simples, resolverlos y combinar los resultados. Ej: Merge Sort. |
| **Algoritmos codiciosos** | Tomar decisiones locales óptimas esperando una solución global óptima. Ej: problema del cambio. |
| **Programación dinámica** | Resolver problemas dividiéndolos en subproblemas que se resuelven una sola vez y se almacenan. Ej: Fibonacci con memoización. |
| **Fuerza bruta**        | Probar todas las posibilidades. Sencillo, pero ineficiente en general. |
| **Backtracking / Recursión** | Probar decisiones parciales y retroceder si no funcionan. Ej: laberintos, Sudoku. |

### 3. **Convertir la estrategia en pseudocódigo**
Un algoritmo debe ser claro y no ambiguo. Es común usar **pseudocódigo** antes de escribir código real.

### 4. **Probar y analizar el algoritmo**
- Validar su **correctitud** con distintos casos (simples, extremos, aleatorios).
- Analizar su **eficiencia** (tiempo y espacio) usando notación asintótica.

---

## ✅ Ejemplo: Potencias con multiplicaciones mínimas

Problema: calcular `x^n` usando el menor número posible de multiplicaciones.

### Estrategia ingenua:
```java
resultado = 1
for i = 1 to n:
    resultado = resultado * x
Tiempo: O(n) multiplicaciones.
```

Estrategia mejorada: Divide y vencerás
```java
POTENCIA(x, n)
    if n == 0:
        return 1
    if n is even:
        y = POTENCIA(x, n/2)
        return y * y
    else:
        return x * POTENCIA(x, n - 1)
```
```java
public class MergeSort {

    // Método para mezclar (merge) dos subarreglos de A[]
    // El primer subarreglo es A[p..q]
    // El segundo subarreglo es A[q+1..r]
    public static void merge(int[] A, int p, int q, int r) {
        int nL = q - p + 1; // longitud del subarreglo izquierdo
        int nR = r - q;     // longitud del subarreglo derecho

        // Crear arreglos temporales para L[] y R[]
        int[] L = new int[nL];
        int[] R = new int[nR];

        // Copiar datos a los arreglos temporales L[] y R[]
        for (int i = 0; i < nL; i++) {
            L[i] = A[p + i];
        }
        for (int j = 0; j < nR; j++) {
            R[j] = A[q + 1 + j];
        }

        // Mezclar los arreglos temporales de nuevo en A[p..r]
        int i = 0; // Índice inicial para L[]
        int j = 0; // Índice inicial para R[]
        int k = p; // Índice inicial para A[]

        while (i < nL && j < nR) {
            if (L[i] <= R[j]) {
                A[k] = L[i];
                i++;
            } else {
                A[k] = R[j];
                j++;
            }
            k++;
        }

        // Copiar los elementos restantes de L[], si hay alguno
        while (i < nL) {
            A[k] = L[i];
            i++;
            k++;
        }

        // Copiar los elementos restantes de R[], si hay alguno
        while (j < nR) {
            A[k] = R[j];
            j++;
            k++;
        }
    }
}
```

![semana3__3](https://github.com/user-attachments/assets/5ee71930-98b4-4ce3-8c00-17b502207878)
![Semana3_](https://github.com/user-attachments/assets/e0e6902c-a238-47bb-841c-fbf7a77f4863)

![semana8](https://github.com/user-attachments/assets/cb420e32-9d1e-4857-be03-58f96974652a)

