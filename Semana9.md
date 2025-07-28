📘 Tema 6: Algoritmos Voraces

Fuente: Brassard, G. & Bratley, P. (2000). Fundamentos de Algoritmos.
🧠 ¿Qué son los Algoritmos Voraces?

Un algoritmo voraz (greedy) es una estrategia de diseño de algoritmos que toma decisiones paso a paso eligiendo la opción que parece mejor en ese momento, sin reconsiderar decisiones pasadas.

    Estrategia localmente óptima: El algoritmo selecciona la mejor opción disponible en cada paso.
    Esperanza de globalmente óptimo: Se espera (aunque no siempre se garantiza) que el resultado final sea el mejor.

⚙️ Características clave

    Construcción paso a paso: Se construye la solución agregando una parte a la vez.
    Sin retroceso: Una vez que se toma una decisión, no se vuelve atrás.
    Eficiencia: Suelen ser algoritmos rápidos y simples.
    Correctitud depende del problema: Solo algunos problemas permiten soluciones óptimas usando esta estrategia.

✅ Problemas donde funciona correctamente

Los algoritmos voraces funcionan bien cuando el problema tiene la propiedad de subestructura óptima y cumple con el criterio de elección voraz.

Ejemplos:

    Problema de la mochila fraccionaria (Fractional Knapsack)
    Árbol de recubrimiento mínimo (Kruskal y Prim)
    Cambio de monedas (cuando las denominaciones permiten solución voraz)
    Selección de actividades (interval scheduling)

🔄 Esquema general del algoritmo voraz

1. Inicializar solución vacía
2. Mientras la solución no sea completa:
    a. Seleccionar la mejor opción según un criterio
    b. Verificar si es factible agregarla
    c. Agregarla a la solución si lo es
3. Devolver la solución final

📉 Limitaciones

    No todos los problemas pueden resolverse de forma óptima con esta estrategia.
    No es adecuado para problemas que requieren considerar combinaciones completas (como el problema de la mochila entera o el viajante).
![Imagen de WhatsApp 2025-07-27 a las 22 30 45_4646ab42](https://github.com/user-attachments/assets/831d5ea1-981d-4bfd-86f7-65a89a8e9878)
![Imagen de WhatsApp 2025-07-27 a las 22 31 01_3efceb8b](https://github.com/user-attachments/assets/edde37c3-76c3-4478-be7f-13a9838295ed)



    
