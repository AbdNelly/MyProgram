#include<iostream>
#include<algorithm>

using namespace std;

int main() {
    int n, i, j, maxkol = 0, kol = 0, l;
    long int a[300010];
    cin >> n;
    for (i = 0; i < n; i++) {
        cin >> a[i];
    }
    sort(a, a + n);
    for (i = 0; i < n; i++) {
        kol = 0;
        for (j = i; j < n; j++) {
            if (a[i] == a[j] && kol < n/2 + 1) {
                kol++;
            } else {
                break;
            }
        }
        if (maxkol <= kol) {
            maxkol = kol;
            l = a[i];
        }
        if (maxkol > n/2) {
            break;
        }
    }
    cout << l;
    return 0;
}
