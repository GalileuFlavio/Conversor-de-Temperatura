# Conversor-de-Temperatura
Um programa que converte temperaturas entre Celsius, Fahrenheit e Kelvin.
#include <stdio.h>

double celsiusParaFahrenheit(double c) {
    return c * 9 / 5 + 32;
}

double celsiusParaKelvin(double c) {
    return c + 273.15;
}

int main() {
    double celsius;
    printf("Digite a temperatura em Celsius: ");
    scanf("%lf", &celsius);

    printf("Fahrenheit: %.2lf\n", celsiusParaFahrenheit(celsius));
    printf("Kelvin: %.2lf\n", celsiusParaKelvin(celsius));

    return 0;
}
