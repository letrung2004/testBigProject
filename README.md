# testBigProject
#include <iostream>
#include<string>
#include <stdlib.h>
#include <json\json.h>
#include <fstream>
using namespace std;
struct dulieu {
	int n;			 // lựa chọn
	int quantity;    // số lượng sản phẩm
	char model;      // model sản phẩm
	int product;     // mã dòng sản phẩm
};
struct dulieu in;

void nhap(int n) {
	//struct dulieu in;
	do
	{
		cout << "========================================\n";
		cout << "*           1. NHAP DON HANG           *\n";
		cout << "*           2. TIM SAN PHAM            *\n";
		cout << "*           3. XUAT DON HANG           *\n";
		cout << "========================================\n";
		cin >> in.n;
		if (in.n > 3 || in.n < 1) {
			cout << "Moi ban nhap lai !\n";
		}


	} while (in.n > 3 || in.n < 1);
}
void nhaphang(int quanlity, char model, int product) {
	cout << "Ma San Pham: - Laptop Dell     (Ma so 1)   | Models San Pham: - Laptop Dell     (Models D)             \n";
	cout << "             - Laptop ASUS     (Ma so 2)   |                  - Laptop ASUS     (Models A)             \n";
	cout << "             - Laptop Lenovo   (Ma so 3)   |                  - Laptop Lenovo   (Models L)             \n";
	cout << "             - Macbook         (Ma so 4)   |                  - Macbook         (Models M)             \n";
	cout << "             - Dt Samsung      (Ma so 5)   |                  - Dt Samsung      (Models S)             \n";
	cout << "             - Dt Iphone       (Ma so 6)   |                  - Dt Iphone       (Models I)             \n";
	cout << "             - Dt Vivo         (Ma so 7)   |                  - Dt Vivo         (Models V)             \n";
	cout << "             - Dt Oppo         (Ma so 8)   |                  - Dt Oppo         (Models O)             \n";

	cout << "Nhap vao ma san pham: "; cin >> in.product;
	cout << "Nhap vao model san pham:"; cin >> in.model;
	cout << "Nhap vao so luong san pham: "; cin >> in.quantity;

}



int main() {
	int n;
	int m;
	nhap(in.n);
	system("cls");
	if (in.n == 1) {
		nhaphang(in.quantity, in.product, in.product);
	}
	for (int i = 0; i < 4; i++)
	{
		cout<<rand() % 10;
	}
	

	cout << endl;
	system("pause");
	return 0;
}
