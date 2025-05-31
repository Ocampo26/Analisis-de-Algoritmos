  # 📘 Capítulo 4.2 – Análisis de las estructuras de control
**Fuente:** Brassard & Bratley – *Fundamentos de Algoritmia*, 2000 (págs. 111–117)

---

## 🎯 Objetivo

Estudiar cómo las **estructuras de control** básicas (secuencias, condicionales e iteraciones) afectan el análisis del tiempo de ejecución de un algoritmo. Este análisis es esencial para estimar la eficiencia computacional de un programa.

---

## 🧱 Estructuras de Control Básicas

### 1. 📜 **Secuencia**

- Cuando varias instrucciones se ejecutan una tras otra.
- El tiempo total es la **suma** del tiempo de cada instrucción.
  
> Ejemplo:  
> Si `I1` toma T₁(n) y `I2` toma T₂(n), entonces  
> **T(n) = T₁(n) + T₂(n)**

---

### 2. 🔁 **Iteración (Bucles)**

#### a) Bucles con número fijo de repeticiones

```java
for i = 1 to n do
    instrucción
```
    Si una instrucción dentro del bucle cuesta O(1) y el bucle va de 1 a n:
    T(n) = O(n)

b) Bucles anidados
```java
for i = 1 to n do
    for j = 1 to n do
        instrucción
```
    Aquí, la instrucción se ejecuta n² veces:
    T(n) = O(n²)

c) Bucles con condición de parada

while condición(n) do
    instrucción

    El análisis depende del número de veces que se ejecuta el cuerpo del bucle.
    Puede depender del peor caso, mejor caso o caso promedio.
    Ejemplo: Búsqueda lineal con ruptura temprana.
        Mejor caso: el primer elemento es el buscado → O(1)
        Peor caso: se recorre toda la lista → O(n)

3. 🔀 Condicionales (if-then-else)
```java
if condición then
    instrucción A
else
    instrucción B
```
    El tiempo de ejecución es el máximo entre ambos caminos:
    T(n) = max(T_A(n), T_B(n))
    En análisis de complejidad, se considera el peor caso.

## Consideraciones Importantes

    Al analizar un algoritmo, se evalúa cada estructura de control individualmente y luego se combinan los tiempos parciales.
    Las funciones de complejidad se expresan en notación asintótica: O(n), O(n²), etc.
    Se pueden hacer suposiciones razonables sobre la entrada para simplificar el análisis.

## Conclusión
    Comprender cómo las estructuras de control influyen en la eficiencia permite escribir algoritmos más rápidos.
    Este análisis es base para evaluar algoritmos más complejos.
    Brassard y Bratley promueven un enfoque sistemático y matemático para el análisis algorítmico.
