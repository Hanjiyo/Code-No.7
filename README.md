#include <iostream>
using namespace std;

int main() {
  int base, exponent, mod, result,x;

  cout << "Enter Base: ";
  cin >> base;
  cout << "Enter exponent: ";
  cin >> ecponent;
  cout << "enter modulo: ";
  cin >> mod;

  result = 1;
  x = base % mod;

  while (exponent > 0) {
    if (exponent % 2 == 1) {
      result = (result * x) % mod;
    }
    x = (x * x) % mod;
    exponent /= 2;
  }

  cout << "Result: "; << result << endl;

  return 0;

}
