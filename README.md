#include <stdio.h>

int main() {
    int age;

    // Ask the user to enter their age
    printf("Enter your age: ");
    if (scanf("%d", &age) != 1) {
        // Check if the input is invalid (not an integer)
        printf("Insufficient data. Please enter a valid number.\n");
        return 1;  // Exit the program
    }

    // Check eligibility for voting
    if (age >= 18) {
        printf("You are eligible for voting. Happy voting!\n");
    } else if (age > 0 && age < 18) {
        printf("You are under age and not eligible for voting.\n");
    } else {
        printf("Invalid age entered. Please enter a positive number.\n");
    }

    return 0;
}
