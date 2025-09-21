#include <iostream>
using namespace std;

int main () {
    int arr[] = {100,300,400,500,600};
    int len = sizeof(arr)/sizeof(arr[0]);
    int *ptr = arr;
    int *ptr1 = arr + len - 1;  
    cout << "Array After reversal: ";
    for (int i = 0; i < len / 2; i++) {
        int temp = *ptr;
        *ptr = *ptr1;
        *ptr1 = temp;
        ptr++;
        ptr1--;
    }
    for (int i = 0; i < len; i++) {
        cout << *(arr + i) << " ";
    }
    cout << endl;
  
    return 0;
}


OUTPUT:
Array After reversal: 600 500 400 300 100
