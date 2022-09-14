# Calculadora-Bhaskara
Calculadora em C de equações de segundo grau (Bháskara)
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main (int argc, char *argv[])
    {
    // Declarar variáveis
    float a, b, c, Delta, x1,x2;

        printf ("Valor A da Expressão:");
    scanf ("%f", &a);
        printf ("Valor B da Expressão:");
    scanf ("%f", &b);
        printf ("Valor C da Expressão:");
    scanf ("%f", &c);
    
    Delta = (b*b) - (4*a*c);
    x1= (-b + sqrt(Delta)) / (2*a);
    x2= (-b - sqrt(Delta)) / (2*a);
    
    
    printf("O valor de Delta: %.2f\n", Delta);
     if (Delta < 0) {
         printf ("Não possui raiz real");
     return 0;
     }
     if(Delta>=0);
        printf("Raiz 1: %2f\n", x1);
     if(Delta>=0);
        printf("Raiz 2: %2f\n", x2);
     return 0;
    }
