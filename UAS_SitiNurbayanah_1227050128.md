# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Siti Nurbayanah
<br>NIM		        :	1227050128
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

  Pada program dari soal pertama Ujian Akhir Semester mata kuliah Dasar Pemrograman kali ini,
  pada soal pertama saya akan membuat program implementasi array 2 dimensi untuk membuat tabel
  bilangan dengan menginputkan jumlah baris dan kolom terlebih dahulu dengan memanfaatkan FOR.
  
  Sedangkan pada soal kedua saya akan mengimplementasikan penggunaan matriks ordo 20x20 pada
  pembuatan tabel dengan kolom dan baris yang juga diinputkan, kemudian dengan menggunakan IF
  ELSE saya membuat program tersebut dapat mencari bilangan kelipatan 3, 5, dan, 7.
  
  Pada pembuatan program kali ini saya menggunakan bahasa C++ dengan tools DevC++.

# Soal 1

## Source Code

#include<iostream>
using namespace std;

int main () {
	
	cout << "=================================================\n";
	cout << "--------------S O A L--N O. 1--U A S-------------\n";
	cout << "=================================================\n\n";
	
	int baris, kolom, bataris, batalom, tasba;
	int batas = baris;
	
	cout << "Masukan Jumlah Baris yang Diinginkan: ";
	cin  >> baris;
	cout << "Masukan Jumlah Kolom yang Diinginkan: ";
	cin  >> kolom;
	cout << endl;
	
	cout << "=================================================\n\n";
	
	int tabel[baris][kolom];
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
			cout << "Masukan nilai koordinat (" << bataris+1 << "," <<batalom+1 << ") : ";
			cin  >> tabel[bataris][batalom];
		}
	}
	
	cout << endl;
	cout << "=================================================\n";
	cout << "------------H A S I L--S O A L--N O. 1-----------\n";
	cout << "=================================================\n\n";
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
		cout << tabel[bataris][batalom] << "\t";
		}
		cout << endl;
	}
	
	cout << endl;
	cout << "=================================================\n";
	cout << "----------H A S I L--P E R U B A H A N-----------\n";
	cout << "=================================================\n\n";
	
	for (batalom = 0; batalom < kolom; batalom++) {
		for (bataris = 0; bataris < baris; bataris++) {
		cout << tabel[bataris][batalom] << "\t";
		}
		cout << endl;
	}
	
	cout << endl;
	cout << "=================================================\n\n";
		
}

# Output

![Screenshot (429)](https://user-images.githubusercontent.com/119025967/209547941-905f0ae0-fef6-429d-b800-3d42d1c4e7cb.png)

# Soal 2

## Source Code

#include <iostream>
using namespace std;

int main() {
	
	cout << "=================================================\n";
	cout << "--------------S O A L--N O. 2--U A S-------------\n";
	cout << "=================================================\n\n";
	
	cout << "Deskripsi :\nBuat pada Matriks 2 dimensi angka-angka (baris kolom diinput),\nlalu menampilkan bilangan yang habis dibagi 3, 5, 7.\n\n";
	
	cout << "=================================================\n\n";
	
	int baris, kolom, bataris, batalom, tasba;
	int batas = baris;
	
	cout << "Masukan Jumlah Baris yang Diinginkan (s/d 20): ";
	cin  >> baris;
	cout << "Masukan Jumlah Kolom yang Diinginkan (s/d 20): ";
	cin  >> kolom;
	cout << endl;
	
	cout << "=================================================\n\n";
	
	int tabel[20][20];
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
			cout << "Masukan nilai koordinat (" << bataris+1 << "," <<batalom+1 << ") : ";
			cin  >> tabel[bataris][batalom];
		}
	}
	
	cout << "=================================================\n\n";
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
			if ( tabel[bataris][batalom] % 3 == 0) {
				cout << "Habis dibagi 3: ";
				cout << tabel[bataris][batalom] << "\n";
			}
			else {
			}
		}
	}
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
			if ( tabel[bataris][batalom] % 5 == 0) {
				cout << "Habis dibagi 5: ";
				cout << tabel[bataris][batalom] << "\n";
			}
			else {
			}
		}
	}
	
	for (bataris = 0; bataris < baris; bataris++) {
		for (batalom = 0; batalom < kolom; batalom++) {
			if ( tabel[bataris][batalom] % 7 == 0) {
				cout << "Habis dibagi 7: ";
				cout << tabel[bataris][batalom] << "\n";
			}
			else {
			}
		}
	}
	
	cout << "=================================================\n\n";
}

## Output

![Screenshot (430)](https://user-images.githubusercontent.com/119025967/209548136-01aed13c-a7fa-40e5-a9ac-ae9a4fcee9b6.png)
	
## Terimakasih
