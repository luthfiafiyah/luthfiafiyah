##Ujian Akhir Semester 

<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Luthfi Afiyah
<br>NIM		        :	1227050065
<br>Jurusan		    : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code

#include<iostream>
using namespace std;


int main()
{
int m, n;

cout << "UJIAN AKHIR SEMESTER"<<endl;
cout << "====================================="<<endl;
cout << " Mata Kuliah	: Dasar Pemrograman"<<endl;
cout << "Nama		: Luthfi Afiyah"<<endl;
cout << "NIM		: 1227050065"<<endl;
cout << "Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung] (https://uinsgd.ac.id/)"<<endl;

cout << "========================================================================================================================"<<endl<<endl;

cout << "No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)" << endl;
cout << "==============================================================="<<endl;
cout << "Masukkan jumlah baris matriks: ";
cin >> m;
cout << "Masukkan jumlah kolom matriks: ";
cin >> n;

int matriks[m][n], transpose[n][m];

cout << "Masukkan Nilai-Nilai Matriks\n";
for (int i = 0; i < m; i++)
{
	for (int j = 0; j < n; j++)
	{
		cout <<"Baris ke "<<i+1<<", Kolom ke "<<j+1<<" : ";
		cin  >> matriks[i][j];
	}
}

cout << endl;
cout << "Hasil dari matriks yang diinputkan :\n";
for (int i = 0; i < m; i++)
{
	for (int j = 0; j < n; j++)
	{
		cout << matriks[i][j] << "\t";
	}
	cout << endl;
}
cout << endl;

for (int i = 0; i < m; i++)
{
	for (int j = 0; j < n; j++)
	{
  		transpose[j][i] = matriks[i][j];
	}
}

cout << "Hasil Transpose Matriks: \n";
for (int i = 0; i < n; i++)
{
	for (int j = 0; j < m; j++)
	{
		cout << transpose[i][j] << "\t";
	}
	cout << endl;
}
cout <<endl;

//buat pada array 2 dimensi angka-angka, menampilkan bilangan yang tidak habis dibagi 3, 5, dan 7  
cout << "No.2 Menampilkan bilangan yang habis dibagi 3, 5 dan 7" << endl;
cout << "==============================================================="<<endl;
cout << "Masukkan jumlah baris matriks: ";
cin >> m;
cout << "Masukkan jumlah kolom matriks: ";
cin >> n;

cout << "Masukkan Nilai-Nilai\n";
for (int i = 0; i < m; i++)
{
	for (int j = 0; j < n; j++)
	{
		cout <<"("<<i+1<<","<<j+1<<") : ";
		cin  >> matriks[i][j];
	}
}
cout << endl;

bool cek = true;
cout << "Nilai yang tidak bisa dibagi 3, 5, 7 yaitu :";
for (int i = 0; i < m; i++)
{
	for (int j = 0; j < n; j++)
	{
		if (matriks[i][j]%3!=0 && matriks[i][j]%5!=0 && matriks[i][j]%7!=0)
		{
			cout << " " << matriks[i][j];
			cek = false;
		}
	}
}
if (cek)
{
	cout << " Nilai yang anda input bisa dibagi 3, 5 dan 7" <<endl;
}
return 0;

}

## Output

UJIAN AKHIR SEMESTER
=====================================
 Mata Kuliah    : Dasar Pemrograman
Nama            : Luthfi Afiyah
NIM             : 1227050065
Jurusan         : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung] (https://uinsgd.ac.id/)
========================================================================================================================

No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)
===============================================================
Masukkan jumlah baris matriks: 2
Masukkan jumlah kolom matriks: 2
Masukkan Nilai-Nilai Matriks
Baris ke 1, Kolom ke 1 : 1
Baris ke 1, Kolom ke 2 : 2
Baris ke 2, Kolom ke 1 : 3
Baris ke 2, Kolom ke 2 : 4

Hasil dari matriks yang diinputkan :
1       2
3       4

Hasil Transpose Matriks:
1       3
2       4

No.2 Menampilkan bilangan yang habis dibagi 3, 5 dan 7
===============================================================
Masukkan jumlah baris matriks: 2
Masukkan jumlah kolom matriks: 2
Masukkan Nilai-Nilai
(1,1) : 1
(1,2) : 2
(2,1) : 3
(2,2) : 4

Nilai yang tidak bisa dibagi 3, 5, 7 yaitu : 1 2 4
--------------------------------
Process exited after 9.658 seconds with return value 0
Press any key to continue . . .
