# Lenguaje-c
# 🧠 Trabajo Práctico – Programación en Lenguaje C

Resolución de 10 ejercicios de lógica en lenguaje C, usando condicionales, estructuras repetitivas y validación de datos.  
Incluye pseudocódigo y código C para cada caso.

---

## ✅ Ejercicio 1: Condicional simple

📌 Leer un número entero y mostrar si es mayor que 100.

**Pseudocódigo:**

Inicio
Leer numero
Si numero > 100 entonces
Escribir "El número es mayor que 100"
FinSi
Fin


**Código en C:**

```c
#include <stdio.h>

int main() {
    int numero;
    printf("Ingrese un número: ");
    scanf("%d", &numero);

    if (numero > 100) {
        printf("El número es mayor que 100.\n");
    }

    return 0;
}


