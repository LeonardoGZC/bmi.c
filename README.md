#include <stdio.h>

int main()
{
    float peso, altura, imc;

    printf("Ingrese su peso en kilogramos: ");
    scanf("%f", &peso);

    printf("Ingrese su altura en metros: ");
    scanf("%f", &altura);

    imc = peso / (altura * altura);

    printf("\nSu índice de masa corporal es: %.2f\n", imc);

    printf("\nTabla de referencia del IMC:\n");
    
    printf(" Categoría               Rango de IMC     \n");
    printf("----------------------------------------\n");
    printf(" Peso bajo               Menos de 18.5    \n");
    printf(" Peso normal             18.5 - 24.9      \n");
    printf(" Sobrepeso               25.0 - 29.9      \n");
    printf(" Obesidad                30.0 o más       \n");
    

    if (imc < 18.5) {
        printf("\nUsted está en la categoría de Peso bajo.\n");
    } else if (imc >= 18.5 && imc <= 24.9) {
        printf("\nUsted está en la categoría de Peso normal.\n");
    } else if (imc >= 25.0 && imc <= 29.9) {
        printf("\nUsted está en la categoría de Sobrepeso.\n");
    } else {
        printf("\nUsted está en la categoría de Obesidad.\n");
    }

    return 0;
    

    
    
}
