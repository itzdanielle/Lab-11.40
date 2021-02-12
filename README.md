# Lab-11.40
#include <iostream>
using namespace std;

int main() {
  double fahrenheit;
  cout << "Enter degrees in Fahrenheit: ";
  cin >> fahrenheit;
  while (fahrenheit < -459.67)
  {
    cout << "Input must be above absolute zero: ";
    cin >> fahrenheit;
  }

  double celsius = (fahrenheit - 32) / 1.8;
  cout << "That temperature in Celsius is " << celsius << endl;

  cout << "Now enter a degrees in Celsius: ";
  cin >> celsius;
  while (celsius < -273.15)
  {
    cout << "Input must be above absolute zero: ";
    cin >> celsius;
  }
  fahrenheit = celsius * 1.8 + 32;
  cout << "That temperature in Fahrenheit is " << fahrenheit << endl;
}
