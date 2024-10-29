#### Bai 1 buoi 1
```c
#include <iostream>
using namespace std;
int main() {
	
	while (true) {
		int n, dem = 0;
		cout << "Nhap vao mot so nguyen duong (-1 de ket thuc): ";
		cin >> n;
		if (n == -1)break;
		while (n != 0) { n /= 10; dem++; }
		cout <<"so "<< n<<" co "<< dem << " ky so " << endl;
	}


}

```
#### Bai 2 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	while (true) {
		int n, max, kyso, min;
		cout << "Nhap vao so nguyen duong (-1 de ket thuc): ";
		cin >> n;
		if (n == -1);
		max = n % 10;
		min = n % 10;
		while (n != 0) {
			kyso = n % 10; n /= 10;
			if (kyso > max)max = kyso;
			else min =kyso;

		}
		cout << "ky so lon nhat la: " << max << endl;
		cout << "ky so nho nhat la: " << min << endl;
	}
}
```
#### Bai 3 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	while (true) {
		int n, daonguoc = 0;
		cout << "Nhap vao mot so nguyen duong (-1 de ket thuc): ";
		cin >> n;
		if (n == -1)break;
		while (n != 0) {
			daonguoc = daonguoc *10+ (n % 10); n /= 10;
		}
			cout << "gia tri dao nguoc la " << daonguoc << endl;
		
	}
}
```
#### Bai 4 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	int n;
	do {
		cout << "Nhap vao mot so nguyen duong (nhap <=0 de dung lai): ";
		cin >> n;
		for (int i = 0; i < n; i++)
			cout << "*" << " " << endl;
		if (n <= 0)break;

	} while (n > 0);
}
```
#### Bai 6 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	int n;
	cout << "Hay nhap vao kich thuoc: ";
	cin >> n;
	for (int i = 1; i <= n; i++) {
		for (int j = 1; j <= n; j++) {
			cout << j * i << " \t";
		}

		cout << endl;
	}
		
}
```
#### Bai 7 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	int n;
	do {
		cout << "Nhap vao mot so nguyen duong (Nhap -1 de ket thuc): ";
		cin >> n;
		for (int i = 1; i <= n; i++) {
			for (int j = 1; j <= n; j++) {
				cout << "*" << " ";
			}
			cout << endl;
		}
	} while (n != -1);
}
```
#### Bai 8 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	int n;
	do {
		cout << "Nhap vao mot so nguyen ( nhap vao -1 de ket thuc): ";
		cin >> n;
		for (int i = 1; i <= n; i++) {
			for (int j = 1; j <= i; j++) {
				cout << "*" << " ";
			}
			cout << endl;
		}
	} while (n != -1);
}
```
#### Bai 9 buoi 1 
```c
#include <iostream>
using namespace std;
int main() {
	int n;
	do {
		cout << "Nhap vao mot so nguyen (nhap -1 de ket thuc): ";
		cin >> n;
		for (int i = 1; i <= n; i++) {
			for (int j = n; j >= i; j--) {
				cout << "*" << " ";
			}
			cout << endl;
		}
	} while (n != -1);
}
```
#### Bai 1 buoi 2
```c
#include <iostream>
#include <conio.h>
using namespace std;
int main() {
	int n;
	cout << "Nhap vao mot so nguyen tu 2 tro len (Nhan phim Esc de dung):";
	cin >> n;
	while (n < 2) {
		cout << "Nhap sai nhap lai: ";
		cin >> n;
	}
	do {
	char c;
		for (int i = 2; i < n; i++) {
			if (n % i == 0)cout << n << " khong phai so nguyen to.";
			else cout << n << " la so nguyen to";
		}
		c = _getch();
		if (c == 27) break;
	} while (true); 
}
```
#### Bai 2 buoi 2
```c
#include <iostream>
using namespace std;
int main() {
	int tu, mau;
		cout << "Chuong trinh nhap vao phan so (nhap mau so bang 0 de ket thuc)!!!" << endl;
		do{cout << "Hay nhap vao tu so: "; cin >> tu;
		cout << "Hay nhap vao mau so: "; cin >> mau;

		int tulate, maulate;
		
			maulate = mau / tu;
			if (mau == 0)tulate = tu;
			else tulate = tu / tu;
			cout << "Vay phan so rut gon cua " << tu << "/" << mau << " la: " << tulate << "/" << maulate<<endl;
		} while (mau != 0);
		
}
```
