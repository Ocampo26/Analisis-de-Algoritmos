# 📘 Comparativo: Divide y vencerás según Cormen (2022) y Brassard & Bratley (2006)

## 🔎 ¿Qué es Divide y Vencerás?

Una **técnica de diseño algorítmico** que resuelve un problema al:
1. **Dividir** el problema en subproblemas más pequeños.
2. **Resolver** recursivamente cada subproblema.
3. **Combinar** las soluciones de los subproblemas en una solución general.

---

## 📗 Cormen et al. (2022) – Capítulo 4: Divide-and-Conquer

### 📌 Estructura de un algoritmo divide y vencerás
```text
DIVIDE:      Dividir el problema en subproblemas más pequeños.
CONQUER:     Resolver recursivamente cada subproblema.
COMBINE:     Combinar soluciones parciales en la solución general.
```
📈 Ejemplos clásicos

    Merge Sort
    Binary Search
    Maximum subarray problem
    Strassen's Matrix Multiplication

🧮 Análisis

    Se usa la recurrencia de tiempo T(n)=aT(n/b)+f(n)T(n)=aT(n/b)+f(n).
    Se resuelve con el Teorema Maestro para obtener la complejidad.

💡 Teorema Maestro

Para T(n)=aT(n/b)+f(n)T(n)=aT(n/b)+f(n), donde:

    a≥1a≥1: número de subproblemas
    b>1b>1: tamaño relativo de los subproblemas
    f(n)f(n): costo de combinar las soluciones

📘 Brassard & Bratley (2006) – Capítulo 7: Divide y Vencerás
🎯 Enfoque didáctico

    Énfasis en el razonamiento paso a paso.
    Usa ejemplos ilustrativos para desarrollar la intuición.

🧠 Ejemplos estudiados

    Ordenación rápida (Quicksort)
    Ordenación por mezcla (Merge Sort)
    Multiplicación de matrices
    Exponenciación rápida
    Problema de la torre de Hanoi

📚 Aplicaciones

    Divide y vencerás se aplica a problemas recursivos que reducen el tamaño del problema en cada paso.
    Se destacan beneficios en paralelismo, claridad algorítmica y análisis eficiente.
![Imagen de WhatsApp 2025-07-27 a las 22 31 53_e7749f76](https://github.com/user-attachments/assets/32cdd8de-bfbf-4b64-843c-cd6ceee5fc61)

![Imagen de WhatsApp 2025-07-27 a las 22 32 04_1b755611](https://github.com/user-attachments/assets/067fb988-09d1-4a1b-b6e0-ac292aab9fec)

    
