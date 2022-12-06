#include <iostream>
using namespace std;

int main() {
	int a[100];
	int n;
	int s = 0 ;
	cin >> n;

	for (int i = 1; i <= n; i++) {
		cin >> a[i];

		for (int j = i; j > 0; j--) {
			if (a[i] < a[j])
				s++;
		}


	}

	
	cout << s;

	return 0;
}
