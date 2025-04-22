#include <iostream>
#include <cmath>
using namespace std;

int main() {
    int temp1, temp2, temp3;

    // Input the temperature readings
    cout << "Enter the first temperature reading: ";
    cin >> temp1;

    cout << "Enter the second temperature reading: ";
    cin >> temp2;

    // Check the increase from first to second reading
    if (temp2 - temp1 > 50) {
        cout << "Reduce fryer heat before taking the third reading." << endl;
        return 0;
    }

    cout << "Enter the third temperature reading: ";
    cin >> temp3;

    // Check the increase from second to third reading
    if (abs(temp3 - temp2) < 10) {
        cout << "Increase the fryer heat before taking the third reading." << endl;
        return 0;
    }

    // Final oil temperature check
    if (temp3 >= 150 && temp3 <= 190) {
        cout << "You may start frying the Magwinyas." << endl;
    } else {
        cout << "Oil is not ready for frying!" << endl;
    }

    return 0;
}
//life then turns upside down
