#include <iostream>
int main() {
    int year;
    std::cout << "Enter a 4-digit year: ";
    std::cin >> year;

    if (year < 1000 || year > 9999) {
        std::cout << "❌ Invalid year. Must be 4 digits.\n";
    } else if ((year % 4 == 0) && (year % 100 != 0 || year % 400 == 0)) {
        std::cout << "✅ That is a leap year.\n";
    } else {
        std::cout << "❌ That is not a leap year.\n";
    }
    return 0;
}

