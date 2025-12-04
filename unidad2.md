➡️ [Regresar al Portafolio Principal](index.md)


# 📂 Unidad 2 – Contenidos y Tareas  

---

## 📘 Contenidos de la Unidad  

- [🔹Estructuras condicionales](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-estructuras-condicionales-tipos-y-ejercicios-en-diagrama-de-flujo-y-en-c)  
  - [🎫 if](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-if)  
  - [🎫 if-else](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-if-else)  
  - [🎫 switch case](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-switch-case)   
- [🔹Estructuras repetitivas](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-estructuras-repetitivas-tipos-y-ejercicios-en-diagrama-de-flujo-y-en-c)  
  - [🎟️ while]()  
  - [🎟️ do...while]()  
  - [🎟️ for]()  
- [🔹Ejercicio combinando](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-ejercicio-combinando-estructura-condicional-y-repetitiva-java-o-python)
  - [🔸Descripción del problema](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#descripci%C3%B3n-del-problema)  
  - [🔸Diagrama de flujo simplificado](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#diagrama-de-flujo-simplificado)  
  - [🔸Programa](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#programa)  
  - [🔸Verificación](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#verificaci%C3%B3n)  
- [🔹Principales dificultades en la aplicación de los contenidos](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-principales-dificultades-en-la-aplicaci%C3%B3n-de-los-contenidos)  
- [🔹Reflexión crítica de los aprendizajes de la unidad](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-reflexi%C3%B3n-cr%C3%ADtica-de-los-aprendizajes-de-la-unidad)  
- [📦 Tareas Entregadas](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#-tareas-entregadas)  
  - [🏠 Aprendizaje Autónomo](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#aprendizaje-aut%C3%B3nomo-aa)  
  - [🪴 Aprendizaje Practico Experimental](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad2.md#aprendizaje-practico-experimental-ape)   
 
---

## 📑 Tabla de ilustraciones  
---

- ## 🔹 **Estructuras condicionales (tipos y ejercicios en diagrama de flujo y en C)**

---

- ### 🎫 if
La sentencia if simple permite ejecutar un bloque de instrucciones solo cuando una condición lógica se cumple. Si la condición es falsa, el programa continúa su ejecución sin realizar ninguna acción adicional asociada al if.
```
if (condicion) {
    // instrucciones si la condición es verdadera
}
```
#### Fig 1: Diagrama de flujo del condicional if simple
<p align="center">
<img width="393" height="245" alt="image" src="https://github.com/user-attachments/assets/aa4128a9-45c8-4015-92c1-601365cff253" />
</p>

---

- ### 🎫 if-else
La estructura IF–ELSE permite ejecutar una acción cuando la condición es verdadera y una acción alternativa cuando es falsa. Si la condición se cumple, se ejecuta el bloque del IF; en caso contrario, se ejecuta el bloque del ELSE.

```
if (condicion) {
    // instrucciones si la condición es verdadera
} else {
    // instrucciones si la condición es falsa
}
```
#### Fig 2: Diagrama de flujo del condicional if-else
<p align="center">
<img width="358" height="204" alt="image" src="https://github.com/user-attachments/assets/c135ea9c-97c4-4cf9-b284-8edba893e321" />
</p>

---

- ### 🎫 switch case
La estructura condicional switch permite evaluar el valor de una variable y ejecutar diferentes bloques de instrucciones según el caso que coincida con ese valor. Cada caso representa una posible opción, y si ninguno coincide, puede definirse un bloque default que se ejecuta como alternativa por defecto.

```
switch (variable) {
    case valor1:
        // instrucciones para valor1
        break;

    case valor2:
        // instrucciones para valor2
        break;

    case valor3:
        // instrucciones para valor3
        break;

    default:
        // instrucciones si no coincide ningún caso
        break;
}
```
#### Fig 3: Diagrama de flujo del condicional switch case
<p align="center">
<img width="487" height="158" alt="image" src="https://github.com/user-attachments/assets/6fd0fcc4-694a-46cd-afed-bc47cee14b63" />
</p>

---

- ## 🔹 **Estructuras repetitivas (tipos y ejercicios en diagrama de flujo y en C)**

---

- ### 🎟️ while
Bucle controlado por condición evaluada antes de ejecutar el cuerpo. Útil cuando no se sabe cuántas veces se repetirá y la ejecución depende de una condición que puede cambiar dentro del bucle. Puede no ejecutarse ninguna vez si la condición es falsa desde el inicio.
```
while (condicion) {
    // instrucciones mientras la condición sea verdadera
}
```
#### Fig 4: Diagrama de flujo del bucle while
<p align="center">
<img width="232" height="204" alt="image" src="https://github.com/user-attachments/assets/20534b01-eb1b-4ca7-85cc-3d03f3512893" />
</p>
---

- ### 🎟️ do...while
Similar a como funciona el bucle while, pero la condición se evalúa después del cuerpo: garantiza que el cuerpo se ejecute al menos una vez. Útil para menús o lectura/validación donde quieres ejecutar la acción antes de comprobar la condición
```
do {
    // instrucciones que se ejecutan al menos una vez
} while (condicion);
```
#### Fig 5: Diagrama de flujo del bucle do...while
<p align="center">
<img width="395" height="359" alt="image" src="https://github.com/user-attachments/assets/4cc28ca5-0c6b-4d5d-9bd2-435fb5537107" />
</p>

---

- ### 🎟️ for
Bucle que se inicializa una variable que actúa como contador, luego se verifica una condición que decide si el ciclo continúa o se detiene, y al final de cada repetición se actualiza el contador. Este proceso se repite automáticamente mientras la condición sea verdadera, lo que permite ejecutar tareas de forma ordenada y controlada cuando ya sabemos cuántas veces deben repetirse.
```
for (inicializacion; condicion; incremento) {
    // instrucciones durante cada iteración
}
```
#### Fig 6: Diagrama de flujo del bucle for
<p align="center">
<img width="354" height="368" alt="image" src="https://github.com/user-attachments/assets/042de146-751e-4683-9be9-9728f0f103ec" />
</p>

---

- ## 🔹 **Ejercicio combinando estructura condicional y repetitiva (Java o Python).**

---

- ### 🔸Descripción del problema  

---

- ### 🔸Diagrama de flujo simplificado  

---

- ### 🔸Programa  

---

- ### 🔸Verificación  

---

## 🔹 **Principales dificultades en la aplicación de los contenidos**  

---

## 🔹 **Reflexión crítica de los aprendizajes de la unidad**  

---

## 📦 Tareas Entregadas  

---

### 🏠Aprendizaje Autónomo (AA)  

---

- ✅ [**AA1: Diferencias entre tipos de estructuras condicionales**](https://drive.google.com/file/d/1hR10PXmLpH3mXsA7WaJdDxKocgz4XCft/view?usp=sharing)  
- ✅ [**AA2: Estructuras algorítmicas de control**](https://drive.google.com/file/d/1VRzeayROfxj-JrlATHLxD7n6hMBdvhmX/view?usp=sharing)  

---

### 🪴Aprendizaje Practico Experimental (APE)  
- ✅ [**APE1: Aplicación de estructuras condicionales en la resolución de problemas.**](https://drive.google.com/file/d/1Rz85MmNwuCmvIG2LT5qjja1AGYhlRgCe/view?usp=sharing)  
- ✅ [**APE2:Aplicación de estructuras repetitivas en la resolución de problemas.**](https://drive.google.com/file/d/1tDZzRGKZr2WPxio06r0gVymwtDkAxUTE/view?usp=drive_link)  


