# Kravchenko_Lab4
#include <iostream>

int main() {
    int numbers[] = {20, 19, 74, 53, 9, 46, 100, 67, 79, 32, 86, 12};
    int size = 12;
    double sum = 0;
    for (int i = 0; i < size; i++) {
        sum += numbers[i];
    }
    double average = sum / size;
    int count = 0;
    for (int i = 0; i < size; i++) {
        if (numbers[i] > average) {
            count++;
        }
    }
    std::cout << "Середнє значення: " << average << std::endl;
    std::cout << "Кількість чисел більших за середнє: " << count << std::endl;

    return 0;
}
