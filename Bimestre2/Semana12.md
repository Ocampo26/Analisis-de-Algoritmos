# 📘 Ordenación por fusión (Merge Sort)

## 📌 Descripción
Merge Sort es un algoritmo de ordenación que usa la técnica **Divide y vencerás**:
- **Divide** el arreglo en mitades hasta obtener subarreglos de tamaño 1.
- **Conquista** (ordena) recursivamente los subarreglos.
- **Combina** las mitades ordenadas en una sola secuencia ordenada.

---

## ⚙️ Pasos del algoritmo

1. **DIVIDE**: Divide el arreglo a la mitad.
2. **CONQUER**: Aplica Merge Sort recursivamente a cada mitad.
3. **MERGE**: Fusiona las dos mitades ordenadas en un solo arreglo ordenado.

---

## 💡 Ejemplo visual

Arreglo: `[38, 27, 43, 3, 9, 82, 10]`

```text
[38, 27, 43, 3, 9, 82, 10]
   /               \
[38, 27, 43, 3]   [9, 82, 10]
... hasta llegar a subarreglos de 1 elemento
... luego fusionamos:
[3, 27, 38, 43]   [9, 10, 82]
y finalmente:
[3, 9, 10, 27, 38, 43, 82]
```
![Imagen de WhatsApp 2025-07-27 a las 22 32 24_93579572](https://github.com/user-attachments/assets/ad906130-b7dc-4602-90c7-4be33b157ebd)

![Imagen de WhatsApp 2025-07-27 a las 22 33 13_a7b7f415](https://github.com/user-attachments/assets/7f445217-bd92-4888-b5c3-50b734f62654)

