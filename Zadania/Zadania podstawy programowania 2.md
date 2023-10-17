```c
#include <stdio.h>
#include <stdlib.h>


void zadanie_1(void) {
    int numbers[3];
    for (int i = 0; i < 3; i++) {
        printf("Podaj liczbe %d:", i+1);
        scanf("%d", &numbers[i]);
    }

    int biggest = numbers[0];
    for (int i = 1; i < 3; i++) {
        if (numbers[i] > biggest) {
            biggest = numbers[i];
        }
    }
    printf("Najwieksza liczba: %d!\n", biggest);
}

void zadanie_2(void) {
    char input[3];

    printf("Podaj znaki:");
    scanf("%c", &input[0]);
    scanf(" %c", &input[1]); // spacja usuwa whitespace z przodu
    scanf(" %c", &input[2]);


    char latest = input[0];
    for (int i = 1; i < 3; i++) {
        if (input[i] > latest) {
            latest = input[i];
        }
    }
    printf("Znak najpozniejszy w alfabecie to %c", latest);
}


void zadanie_3(void) {

    int input_a;
    int input_b;

    unsigned char a;
    unsigned char b;
    // scanf spacja przed = odciecie whitespace

    printf("Enter a:\n");
    scanf("%d", &input_a);

    printf("Enter b:\n");
    scanf("%d", &input_b);
    a = (unsigned char) input_a;
    b = (unsigned char) input_b;


    printf("a, b = %x, %x (%d, %d)\n", a, b, a, b);
    printf("a & b = %x (%d)\n", a&b, a&b);
    printf("a | b = %x (%d)\n", a|b, a|b);
    printf("a ^ b = %x (%d)\n", a^b, a^b);

}


void zadanie_4(void) {
    int a;
    short int b;
    double c;
    printf("a=%d, b=%hu, c=%lf", a, b, c);
}

void zadanie_5(void) {
    int a, b;
    printf("Enter a:");
    scanf("%d", &a);
    printf("Enter b:");
    scanf("%d", &b);

    printf("%d / %d = %d\n", a, b, a / b);
}
void zadanie_6(void) {
    int a, b;
    printf("Enter a:");
    scanf("%d", &a);
    printf("Enter b:");
    scanf("%d", &b);

    if (a % b == 0) {
        printf("%d\n", a);
    }
    else {
        printf("%d\n", b);
    }
}

void zadanie_7(void) {
    int a;
    printf("Enter a:");
    scanf("%d", &a);

    if( a - (2 * (a/2)) ) {
        printf("Liczba jest nieparzysta.\n");
    }
    else {
        printf("Liczba jest parzysta.\n");
    }
}

void zadanie_8(void) {
    unsigned char x;
    x = x - 1;
    printf("%d\n", x);
}

// zadanie_9(todo)

int main()
{
    zadanie_8();
    return 0;
}

```


[[formaty w c]]