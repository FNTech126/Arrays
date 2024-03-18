# Arrays

#include <iostream>

using namespace std;

const int ROWS = 3;
const int COLS = 3;

int main() {
    int array[ROWS][COLS];

    // Input data into the array
    cout << "Enter " << ROWS * COLS << " elements for the array:" << endl;
    for (int i = 0; i < ROWS; ++i) {
        for (int j = 0; j < COLS; ++j) {
            cout << "Enter element at position (" << i << "," << j << "): ";
            cin >> array[i][j];
        }
    }

    // Output the contents of the array
    cout << "\nContents of the array:" << endl;
    for (int i = 0; i < ROWS; ++i) {
        for (int j = 0; j < COLS; ++j) {
            cout << array[i][j] << " ";
        }
        cout << endl;
    }

    return 0;
}
