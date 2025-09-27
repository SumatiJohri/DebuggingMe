# DebuggingMe
Plethora of codes, certificates and experiences of different coding courses and events.
#include <stdio.h>
int main() {
    float num1, num2;
    printf("Enter first number: ");
    scanf("%f", &num1);
    printf("Enter second number: ");
    scanf("%f", &num2);
    int choice;
    printf("\nSIMPLE CALCULATOR\n");
    for (int i=0; i<1; i++) {
        printf("1. Addition\n");
        printf("2. Subtraction\n");
        printf("3. Multiplication\n");
        printf("4. Division\n");
        printf("5. Exiting Calculator\n");
    }
    printf("Enter choice->");
    scanf("%d", &choice);
    switch(choice) {
        case 1:
        printf("%.2f + %.2f = %.2f\n", num1, num2, num1+num2);
        break;
        case 2:
        printf("%.2f - %.2f = %.2f\n", num1, num2, num1-num2);
        break;
        case 3:
        printf("%.2f * %.2f = %.2f\n", num1, num2, num1/num2);
        break;
        case 4:
        if (num2==0) {
            printf("Error! Division by zero");
        }
        else {
            printf("%.2f \ %.2f = %.2f\n", num1, num2, num1/num2);
        }
        break;
        default:
        printf("Invalid choice");
    }
    return 0;
}
