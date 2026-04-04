#include <stdio.h>

int main() {
    int a, b;
    char op;

    printf("===== Simple C Calculator =====\n");

    printf("Enter first number: ");
    scanf("%d", &a);

    printf("Enter second number: ");
    scanf("%d", &b);

    printf("Enter operator (+, -, *, /): ");
    scanf(" %c", &op);

    if (op == '+') {
        printf("Result = %d\n", a + b);
    }
    else if (op == '-') {
        printf("Result = %d\n", a - b);
    }
    else if (op == '*') {
        printf("Result = %d\n", a * b);
    }
    else if (op == '/') {
        if (b != 0) {
            printf("Result = %d\n", a / b);
        } else {
            printf("Error: Cannot divide by zero\n");
        }
    }
    else {
        printf("Invalid operator\n");
    }

    return 0;
}
