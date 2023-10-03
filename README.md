# examen2

codigo 1

#include <iostream>

int main() {
    int year;

    std::cout << "Ingrese un ano: ";
    std::cin >> year;

    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        std::cout << year << " es un ano bisiesto." << std::endl;
    } else {
        std::cout << year << " no es un ano bisiesto." << std::endl;
    }

    return 0;
}


codigo 2

#include <iostream>

int main() {
    int altura;

    // Solicitar al usuario la altura de la pirámide
    std::cout << "Ingrese la altura de la piramide: ";
    std::cin >> altura;

    for (int i = 1; i <= altura; i++) {
        for (int j = 1; j <= i; j++) {
            std::cout << j << " ";
        }
        std::cout << std::endl;
    }

    return 0;
}


codigo 3

#include <iostream>

int main() {
    int numero;

    std::cout << "Ingrese un numero: ";
    std::cin >> numero;

    if (numero % 3 == 0) {
        std::cout << numero << " es multiplo de 3." << std::endl;
    } else {

    codigo 4

    #include <stdio.h> 

int main() {
    int n1, n2, resultado, suma;
    
    printf("Introduzca un numero:\n");
    scanf("%d", &n1);
    
    printf("Introduzca otro numero:\n");
    scanf("%d", &n2);
    
    resultado = n1 + n2; 
    
    printf("Cuanto suman?:\n");
    scanf("%d", &suma);
    
    if (suma == resultado) { 
        printf("Correcto\n");
    } else {
        printf("INCORRECTO: La suma es %d\n", resultado); 
    }
    
    return 0;
}
        std::cout << numero << " no es multiplo de 3." << std::endl;
    }

    return 0;
}
