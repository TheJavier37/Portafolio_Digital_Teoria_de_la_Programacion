[Volver a Tareas entregadas](https://github.com/TheJavier37/Portafolio_Digital_Teoria_de_la_Programacion/blob/main/unidad3.md#-tareas-entregadas)
```c
#include <stdio.h>

void calcularValorCliente(float *totalRecaudado);
void calcularValorRecaudado(int numeroClientes);

int main() {
    int numeroClientes;

    printf("Ingrese el numero de clientes: ");
    scanf("%i", &numeroClientes);
  
    calcularValorRecaudado(numeroClientes);

    return 0;
}

void calcularValorRecaudado(int numeroClientes) {
    int i;
    float totalRecaudado = 0;

    for(i = 1; i <= numeroClientes; i++){
        calcularValorCliente(&totalRecaudado);
    }

    printf("El valor total recaudado es: %.2f\n", totalRecaudado);
}

void calcularValorCliente(float *totalRecaudado) {
    int tipoConsola;
    int tiempoJuego;
    float tarifa;
    float valorCliente;
  
    do {
        printf("\nIngrese el tipo de consola:\n");
        printf("1 = PlayStation\n");
        printf("2 = Xbox\n");
        printf("3 = Nintendo\n");
        scanf("%i", &tipoConsola);

        if(tipoConsola < 1 || tipoConsola > 3){
            printf("Error, ingrese un numero valido\n");
        }

    } while(tipoConsola < 1 || tipoConsola > 3);

    if(tipoConsola == 1){
        tarifa = 2.50;
    } else if(tipoConsola == 2){
        tarifa = 2.00;
    } else {
        tarifa = 1.50;
    }

    printf("Ingrese el tiempo de juego: ");
    scanf("%i", &tiempoJuego);

    valorCliente = tarifa * tiempoJuego;

    *totalRecaudado += valorCliente;
}
```
