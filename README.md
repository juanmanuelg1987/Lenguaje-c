# Lenguaje-c
# 🧠 Trabajo Práctico – Programación en Lenguaje C

Resolución de 10 ejercicios de lógica en lenguaje C, usando condicionales, estructuras repetitivas y validación de datos.  
Incluye pseudocódigo y código C para cada caso.

---

## ✅ Ejercicio 1: Condicional simple

 Leer un número entero y mostrar si es mayor que 100.

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


✅ Ejercicio 2: Condicional doble (if-else)
 Leer una edad e indicar si la persona es mayor o menor de edad.

Pseudocódigo:
Inicio
    Leer edad
    Si edad >= 18 entonces
        Escribir "Mayor de edad"
    Sino
        Escribir "Menor de edad"
    FinSi
Fin


#include <stdio.h>

int main() {
    int edad;
    printf("Ingrese su edad: ");
    scanf("%d", &edad);

    if (edad >= 18) {
        printf("Mayor de edad.\n");
    } else {
        printf("Menor de edad.\n");
    }

    return 0;
}


✅ Ejercicio 3: Condicional múltiple (if - else if)
Ingresar una nota del 1 al 10 y mostrar:

“Insuficiente” si es menor que 6.

“Suficiente” si es 6 o 7.

“Bueno” si es 8 o 9.

“Excelente” si es 10.

Pseudocódigo:
Inicio
    Leer nota
    Si nota < 6 entonces
        Escribir "Insuficiente"
    Sino si nota <= 7 entonces
        Escribir "Suficiente"
    Sino si nota <= 9 entonces
        Escribir "Bueno"
    Sino si nota == 10 entonces
        Escribir "Excelente"
    FinSi
Fin
Código en C:

#include <stdio.h>

int main() {
    int nota;
    printf("Ingrese una nota (1-10): ");
    scanf("%d", &nota);

    if (nota < 6) {
        printf("Insuficiente.\n");
    } else if (nota <= 7) {
        printf("Suficiente.\n");
    } else if (nota <= 9) {
        printf("Bueno.\n");
    } else if (nota == 10) {
        printf("Excelente.\n");
    }

    return 0;
}


✅ Ejercicio 4: Estructura for
 Mostrar los números del 1 al 10 usando un bucle for.

Pseudocódigo:
Inicio
    Para i desde 1 hasta 10 hacer
        Escribir i
    FinPara
Fin

Código en C:

#include <stdio.h>

int main() {
    for (int i = 1; i <= 10; i++) {
        printf("%d\n", i);
    }

    return 0;
}


✅ Ejercicio 5: Estructura while
 Leer números hasta ingresar un 0. Al finalizar, mostrar cuántos números se ingresaron.

Pseudocódigo:
Inicio
    contador ← 0
    Leer numero
    Mientras numero ≠ 0 hacer
        contador ← contador + 1
        Leer numero
    FinMientras
    Escribir "Cantidad de números ingresados: ", contador
Fin
Código en C:


#include <stdio.h>

int main() {
    int numero, contador = 0;
    printf("Ingrese un número (0 para terminar): ");
    scanf("%d", &numero);

    while (numero != 0) {
        contador++;
        printf("Ingrese otro número (0 para terminar): ");
        scanf("%d", &numero);
    }

    printf("Se ingresaron %d números.\n", contador);
    return 0;
}


✅ Ejercicio 6: Estructura do-while
Repetir el ingreso de una clave hasta que el usuario escriba “1234”. Mostrar un mensaje de bienvenida al ingresar correctamente.

Pseudocódigo:

Inicio
    Repetir
        Leer clave
    Hasta que clave = 1234
    Escribir "Bienvenido"
Fin

Código en C:

#include <stdio.h>

int main() {
    int clave;

    do {
        printf("Ingrese la clave: ");
        scanf("%d", &clave);
    } while (clave != 1234);

    printf("¡Bienvenido!\n");
    return 0;
}


✅ Ejercicio 7: Contadores y acumuladores
Leer 5 números enteros. Mostrar la suma total y cuántos eran positivos.

Pseudocódigo:

nginx
Copiar
Editar
Inicio
    suma ← 0
    positivos ← 0
    Para i desde 1 hasta 5 hacer
        Leer numero
        suma ← suma + numero
        Si numero > 0 entonces
            positivos ← positivos + 1
        FinSi
    FinPara
    Escribir "Suma total: ", suma
    Escribir "Cantidad de positivos: ", positivos
Fin

Código en C:

#include <stdio.h>

int main() {
    int numero, suma = 0, positivos = 0;

    for (int i = 1; i <= 5; i++) {
        printf("Ingrese un número: ");
        scanf("%d", &numero);
        suma += numero;
        if (numero > 0) {
            positivos++;
        }
    }

    printf("Suma total: %d\n", suma);
    printf("Cantidad de positivos: %d\n", positivos);
    return 0;
}


✅ Ejercicio 8: Validación de entrada
Pedir una nota entre 1 y 10. Si se ingresa un número inválido, volver a pedir.

Pseudocódigo:

Inicio
    Repetir
        Leer nota
    Hasta que nota ≥ 1 y nota ≤ 10
    Escribir "Nota válida: ", nota
Fin

Código en C:
#include <stdio.h>

int main() {
    int nota;

    do {
        printf("Ingrese una nota (1-10): ");
        scanf("%d", &nota);
    } while (nota < 1 || nota > 10);

    printf("Nota válida: %d\n", nota);
    return 0;
}


✅ Ejercicio 9: Tabla de multiplicar
Pedir un número e imprimir su tabla de multiplicar del 1 al 10.

Pseudocódigo:
Inicio
    Leer numero
    Para i desde 1 hasta 10 hacer
        Escribir numero * i
    FinPara
Fin

Código en C:
#include <stdio.h>

int main() {
    int numero;

    printf("Ingrese un número: ");
    scanf("%d", &numero);

    for (int i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", numero, i, numero * i);
    }

    return 0;
}


✅ Ejercicio 10: Conteo de pares e impares
Leer 10 números e indicar cuántos son pares y cuántos impares.

Pseudocódigo:

Inicio
    pares ← 0
    impares ← 0
    Para i desde 1 hasta 10 hacer
        Leer numero
        Si numero mod 2 = 0 entonces
            pares ← pares + 1
        Sino
            impares ← impares + 1
        FinSi
    FinPara
    Escribir "Pares: ", pares
    Escribir "Impares: ", impares
Fin

Código en C:

#include <stdio.h>

int main() {
    int numero, pares = 0, impares = 0;

    for (int i = 1; i <= 10; i++) {
        printf("Ingrese un número: ");
        scanf("%d", &numero);

        if (numero % 2 == 0) {
            pares++;
        } else {
            impares++;
        }
    }

    printf("Cantidad de pares: %d\n", pares);
    printf("Cantidad de impares: %d\n", impares);
    return 0;
}
