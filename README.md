#include <stdio.h>

// Recursive function to solve Tower of Hanoi
void towerOfHanoi(int n, char source, char auxiliary, char destination) {
    if (n == 1) {
        printf("Move disk 1 from %c → %c\n", source, destination);
        return;
    }

    // Move (n-1) disks from source to auxiliary
    towerOfHanoi(n - 1, source, destination, auxiliary);

    // Move the largest disk from source to destination
    printf("Move disk %d from %c → %c\n", n, source, destination);

    // Move (n-1) disks from auxiliary to destination
    towerOfHanoi(n - 1, auxiliary, source, destination);
}

int main() {
    int n;

    printf("Enter number of disks: ");
    scanf("%d", &n);

    printf("\nSteps to solve Tower of Hanoi:\n\n");
    towerOfHanoi(n, 'A', 'B', 'C');

    printf("\nTotal number of moves: %d\n", (1 << n) - 1); // 2^n - 1 formula

    return 0;
}


