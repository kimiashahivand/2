#include <iostream>
using namespace std;

int max(int a, int b) {
    return (a > b) ? a : b;
}

int max(int a, int b, int c, int d) {
    return max(max(a, b), max(c, d));
}

int main() {
    int a, b, c, d;
    cout << "Enter 4 integers: ";
    cin >> a >> b >> c >> d;
    cout << "Maximum is: " << max(a, b, c, d) << endl;
    return 0;
}
