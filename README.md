# prime-num-between-1-to-100 in c program
#include <stdio.h>
int main() {
    int i, j, isPrime;

    for (i = 2; i <= 100; i++) {
        isPrime = 1;
        for (j = 2; j * j <= i; j++) {
            if (i % j == 0) {
                isPrime = 0;
                break;
            }
        }
        if (isPrime) {
            printf("%d ", i);
        }
    }

    return 0;
}
