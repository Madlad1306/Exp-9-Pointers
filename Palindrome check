#include <iostream>
#include <cstring>
using namespace std;

int main() {
    char str[100];
    cout << "Enter a string: ";
    cin >> str;

    char *start = str;
    char *end = str + strlen(str) - 1;

    bool isPalindrome = true;

    while (start < end) {
        if (*start != *end) {
            isPalindrome = false;
            break;
        }
        start++;
        end--;
    }

    if (isPalindrome)
        cout << "The string is a palindrome." << endl;
    else
        cout << "The string is not a palindrome." << endl;

    return 0;
}


OUTPUT :

Enter a string: madam
The string is a palindrome.
Enter a string: hello
The string is not a palindrome.
