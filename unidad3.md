➡️ [Regresar al Portafolio Principal](index.md)


# 📂 Unidad 3 – Contenidos y Tareas  

---

## 📘 Contenidos de la Unidad

- [🔹 Modularidad](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-modularidad)  
    ▪ [🔸Ejemplo de Modularidad con Paso de Parámetros](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#ejemplo-de-modularidad-con-paso-de-par%C3%A1metros)  
    ▪ [🔸Ejemplo de Modularidad con Paso de Referencias](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#ejemplo-de-modularidad-con-paso-de-referencias)
      
- [🔹 Arreglos](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-arreglos)  
    ▪ [🔸Ejemplo de Arreglo Unidimensional](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#ejemplo-de-arreglo-unidimensional)  
    ▪ [🔸Ejemplo de Arreglo Bidimensional](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#ejemplo-de-arreglo-bidimensional)  
    ▪ [🔸Ejemplo de Arreglo Tridimensional](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#ejemplo-de-arreglo-tridimensional)  
    
- [🔹 Principales dificultades en la aplicación de los contenidos](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-principales-dificultades-en-la-aplicaci%C3%B3n-de-los-contenidos)  
- [🔹 Reflexión crítica de los aprendizajes de la unidad](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-reflexi%C3%B3n-cr%C3%ADtica-de-los-aprendizajes-de-la-unidad)  
- [📦 Tareas Entregadas](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-tareas-entregadas)  

---

- ## 🔹 **Modularidad**

La **modularidad en la programación** es un principio que consiste en **dividir un programa grande en partes más pequeñas e independientes**, llamadas **módulos**, donde cada una cumple una función específica.

En lugar de tener todo el código en un solo bloque, se organiza en componentes bien definidos como **funciones, clases, archivos o paquetes**.

### ¿Qué es un módulo?
Un **módulo** es una pieza de código que:
- Tiene una **responsabilidad clara**
- Puede **usarse, probarse o modificarse** sin afectar todo el programa
- Se comunica con otros módulos mediante **interfaces claras**

### Ejemplo sencillo
En una aplicación típica se pueden tener:
- Módulo de **inicio de sesión**
- Módulo de **cálculos**
- Módulo de **interfaz de usuario**
- Módulo de **base de datos**

Cada módulo cumple su función específica sin interferir con los demás.

### Importancia de la modularidad
La modularidad permite:
- Facilitar el **mantenimiento** del código
- Promover la **reutilización** de componentes
- Mejorar la **legibilidad y organización**
- Detectar y corregir **errores** más rápidamente
- Permitir el **trabajo en equipo** de forma más eficiente
  
## 🔸Ejemplo de Modularidad con Paso de Parámetros

### Contexto

El programa principal solicita tres calificaciones al usuario y las envía como **parámetros** a una **función modular**, la cual se encarga de realizar el cálculo del promedio y devolver el resultado al programa principal. Este enfoque permite separar el proceso de entrada de datos del cálculo, promoviendo un código más organizado, reutilizable y fácil de mantener.


```c
#include <stdio.h>

/* Función modular que recibe parámetros */
float calcularPromedio(float nota1, float nota2, float nota3) {
    float promedio;
    promedio = (nota1 + nota2 + nota3) / 3;
    return promedio;
}

int main() {
    float calificacion1, calificacion2, calificacion3;
    float resultado;

    /* Entrada de datos */
    printf("Ingrese la primera calificacion: ");
    scanf("%f", &calificacion1);

    printf("Ingrese la segunda calificacion: ");
    scanf("%f", &calificacion2);

    printf("Ingrese la tercera calificacion: ");
    scanf("%f", &calificacion3);

    /* Llamada al módulo pasando parámetros */
    resultado = calcularPromedio(calificacion1, calificacion2, calificacion3);

    /* Salida */
    printf("El promedio es: %.2f\n", resultado);

    return 0;
}

```

----

## 🔸Ejemplo de Modularidad con Paso de Referencias
### Contexto del ejercicio

Se desea desarrollar un programa que calcule el **promedio de tres calificaciones** de un estudiante aplicando el principio de **modularidad**.  
Para ello, el cálculo se realizará en una **función independiente** que no devolverá un valor directamente, sino que **modificará una variable del programa principal mediante paso de referencia**.

Este enfoque permite que la función tenga la capacidad de **alterar datos externos**, demostrando el uso de **punteros en el lenguaje C** y favoreciendo una mejor organización, reutilización y claridad del código.

```c
#include <stdio.h>

/* Función modular con paso de referencia */
void calcularPromedio(float nota1, float nota2, float nota3, float *promedio) {
    *promedio = (nota1 + nota2 + nota3) / 3;
}

int main() {
    float calificacion1, calificacion2, calificacion3;
    float resultado;

    /* Entrada de datos */
    printf("Ingrese la primera calificacion: ");
    scanf("%f", &calificacion1);

    printf("Ingrese la segunda calificacion: ");
    scanf("%f", &calificacion2);

    printf("Ingrese la tercera calificacion: ");
    scanf("%f", &calificacion3);

    /* Llamada a la función pasando la referencia */
    calcularPromedio(calificacion1, calificacion2, calificacion3, &resultado);

    /* Salida */
    printf("El promedio es: %.2f\n", resultado);

    return 0;
}

```

---

- ## 🔹 **Arreglos**

Los **arreglos** (también llamados **arrays**) son estructuras de datos que permiten **almacenar múltiples valores del mismo tipo** bajo un solo nombre.

Cada valor dentro del arreglo se identifica mediante un **índice**, que indica su posición.

### Características de los arreglos
- Almacenan **varios datos del mismo tipo**
- Tienen un **tamaño definido**
- Cada elemento se accede mediante un **índice**
- Los índices normalmente comienzan desde **0**
- Permiten acceso **rápido y directo** a los elementos

### Ejemplo conceptual
Un arreglo de números puede representar:
- Calificaciones de un estudiante
- Edades de un grupo de personas
- Precios de productos

Ejemplo de posiciones:
- Índice 0 → Primer elemento  
- Índice 1 → Segundo elemento  
- Índice 2 → Tercer elemento  

### Tipos de arreglos
- **Unidimensionales**: almacenan datos en una sola fila.
- **Bidimensionales**: organizan los datos en filas y columnas (matrices).
- **Tridimensionales**: que pueden interpretarse como capas, filas y columnas.

### Ventajas de los arreglos
- Facilitan el **manejo de grandes cantidades de datos**
- Reducen la cantidad de **variables necesarias**
- Permiten realizar **operaciones repetitivas** de forma eficiente

### Desventajas de los arreglos
- Su tamaño suele ser **fijo**
- No son ideales cuando se requiere **insertar o eliminar** elementos con frecuencia

## 🔸Ejemplo de Arreglo Unidimensional
### Contexto
Se utiliza un arreglo unidimensional para almacenar y mostrar cinco calificaciones ingresadas por el usuario.
### Código en C
```c
#include <stdio.h>

int main() {
    int calificaciones[5];
    int i;

    for (i = 0; i < 5; i++) {
        printf("Ingrese la calificacion %d: ", i + 1);
        scanf("%d", &calificaciones[i]);
    }

    printf("\nCalificaciones ingresadas:\n");
    for (i = 0; i < 5; i++) {
        printf("%d ", calificaciones[i]);
    }

    return 0;
}

```
📌 Uso principal: listas simples (edades, notas, precios).

---

## 🔸Ejemplo de Arreglo Bidimensional
### Contexto

Se utiliza un arreglo bidimensional para representar una matriz 2x3, útil para manejar datos organizados en filas y columnas.

Código en C

```c
#include <stdio.h>

int main() {
    int matriz[2][3];
    int i, j;

    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            printf("Ingrese el valor [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
        }
    }

    printf("\nMatriz ingresada:\n");
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d ", matriz[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```
📌 Uso principal: tablas, matrices matemáticas, registros organizados.

---

## 🔸Ejemplo de Arreglo Tridimensional
### Contexto
Se emplea un arreglo tridimensional para almacenar datos en tres dimensiones, por ejemplo: calificaciones de 2 estudiantes, en 2 materias, con 3 evaluaciones cada una.
```c
#include <stdio.h>

int main() {
    int notas[2][2][3];
    int i, j, k;

    for (i = 0; i < 2; i++) {
        for (j = 0; j < 2; j++) {
            for (k = 0; k < 3; k++) {
                printf("Estudiante %d, Materia %d, Evaluacion %d: ",
                       i + 1, j + 1, k + 1);
                scanf("%d", &notas[i][j][k]);
            }
        }
    }

    printf("\nNotas registradas:\n");
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 2; j++) {
            for (k = 0; k < 3; k++) {
                printf("%d ", notas[i][j][k]);
            }
            printf("\n");
        }
        printf("\n");
    }

    return 0;
}
```
📌 Uso principal: simulaciones, datos complejos, estructuras de varios niveles.

---

## 🔹 **Principales dificultades en la aplicación de los contenidos**  

👁️ En la modularidad un diseño incorrecto de los módulos o un exceso de dependencias puede complicar el mantenimiento del programa, además de que el manejo inadecuado del paso de parámetros, especialmente entre valor y referencia, suele generar errores lógicos difíciles de detectar.  
📁 Por otro lado, en el uso de arreglos, los errores de índice, la definición incorrecta del tamaño, la falta de inicialización y la complejidad de los arreglos multidimensionales pueden provocar fallos en la ejecución y un uso ineficiente de la memoria, por lo que ambos conceptos requieren una correcta planificación y atención al detalle para aplicarse de manera efectiva.  

---

## 🔹 **Reflexión crítica de los aprendizajes de la unidad**  

📖 El aprendizaje sobre la programación modular y el uso de arreglos permitió comprender la importancia de organizar el código de manera estructurada y lógica, facilitando su lectura, mantenimiento y reutilización.  
🧠 Asimismo, el manejo de arreglos ayudó a entender cómo almacenar y procesar grandes cantidades de datos de forma eficiente, reforzando el cuidado en el uso de índices y memoria. En conjunto, estos conceptos fortalecen el pensamiento lógico y la capacidad de diseñar soluciones más ordenadas y escalables dentro del desarrollo de programas, como se esta aplicando en el proyecto integrador.  

---

## 📦 Tareas Entregadas  

### 🏠Aprendizaje Autónomo (AA)  

- ✅ [**AA1: Curso Python Essencials 1**](https://drive.google.com/file/d/1meeLsqiw6PQh4CAJI6I2t-HMdao5h3oq/view?usp=drive_link)   

### 🪴Aprendizaje Practico Experimental (APE)  
- ✅ [**APE1: Construcción de funciones y procedimientos en un lenguaje de programación.**](https://drive.google.com/file/d/1T2wC6GtiAJBB3j37UKlwXFVD6YI18aTi/view?usp=sharing)  
- ✅ [**APE2: Implementación de funciones utilizando el paso de parámetros por valor y por referencia:**](replitu3.md)


