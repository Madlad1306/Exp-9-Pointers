#include <iostream>
using namespace std;

int main() {
    int Arr[] = {100, 200, 400, 500, 600};
    int sum = 0;
    int* ptr = Arr;
    
    for (int i = 0; i < 5; i++) {
        sum += *(ptr + i);
    }
    cout << "Sum of Array Elements : " << sum << endl;  

    int *prt1 = &Arr[0];
    int *ptr2 = &Arr[4];
    int diff = *ptr2 - *prt1;
    cout << "Difference between first and last element pointers: " << diff << endl;
    return 0;
}


OUTPUT : 
Sum of Array Elements : 1800
Difference between first and last element pointers: 500
