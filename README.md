# Codeforcescpp-31A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int n, arr[100], sum, index;
	cin >> n;
	for (int i = 0; i < n; i++) {
		cin >> arr[i];
	}
	for (int i = 0; i < n - 1; i++) {
		for (int j = i + 1; j < n; j++) {
			sum = arr[i] + arr[j];
			for (int k = 0; k < n; k++) {
				if (sum == arr[k]) {
					cout << k + 1 << " " << i + 1 << " " << j + 1;
					return 0;
				}
			}
		}
	}
cout << -1;
return 0;
}
