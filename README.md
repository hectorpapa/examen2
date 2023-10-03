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
