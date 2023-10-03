# examen2

codigo 1

#include <iostream>
#include <cstdlib> 
#include <ctime>   
#include <cmath> 

int main() {
    std::srand(static_cast<unsigned int>(std::time(nullptr)));
    int numeroAleatorio = (std::rand() % 5) + 1;
    std::cout << "Número aleatorio: " << numeroAleatorio << std::endl;

    switch (numeroAleatorio) {
        case 1:
        {
            double numero1, numero2;
            std::cout << "Ingrese el primer número: ";
            std::cin >> numero1;
            std::cout << "Ingrese el segundo número: ";
            std::cin >> numero2;
            double suma = numero1 + numero2;
            std::cout << "La suma de " << numero1 << " y " << numero2 << " es: " << suma << std::endl;
            break;
        }
        case 2:
        {
            double numero1, numero2;
            std::cout << "Ingrese el primer número: ";
            std::cin >> numero1;
            std::cout << "Ingrese el segundo número: ";
            std::cin >> numero2;
            double resta = numero1 - numero2;
            std::cout << "La resta de " << numero1 << " y " << numero2 << " es: " << resta << std::endl;
            break;
        }
        case 3:
        {
            double numero1, numero2;
            std::cout << "Ingrese el primer número: ";
            std::cin >> numero1;
            std::cout << "Ingrese el segundo número: ";
            std::cin >> numero2;
            double multiplicacion = numero1 * numero2;
            std::cout << "La multiplicación de " << numero1 << " y " << numero2 << " es: " << multiplicacion << std::endl;
            break;
        }
        case 4:
        {
            double dividendo, divisor;
            std::cout << "Ingrese el dividendo: ";
            std::cin >> dividendo;
            std::cout << "Ingrese el divisor: ";
            std::cin >> divisor;
            if (divisor == 0) {
                std::cout << "Error: No se puede dividir por cero." << std::endl;
            } else {
                double resultado = dividendo / divisor;
                std::cout << "El resultado de la división es: " << resultado << std::endl;
            }
            break;
        }
        case 5:
        {
            double numero;
            std::cout << "Ingrese un número para calcular su raíz cuadrada: ";
            std::cin >> numero;
            if (numero < 0) {
                std::cout << "Error: No se puede calcular la raíz cuadrada de un número negativo." << std::endl;
            } else {
                double raizCuadrada = std::sqrt(numero);
                std::cout << "La raíz cuadrada de " << numero << " es: " << raizCuadrada << std::endl;
            }
            break;
        }
        default:
            std::cout << "Número no válido" << std::endl;
            break;
    }

    return 0;
}
