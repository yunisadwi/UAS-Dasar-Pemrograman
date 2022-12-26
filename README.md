# Ujian Akhir Semester 

<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Yunisa Dwi Indrayani
<br>NIM		        :	1227050135
<br>Jurusan	    	: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 


##Deskripsi Umum
<br>Array adalah variabel yang mempunyai indeks sehingga dapat menyimpan sejumlah data yang bertipe sama. Dimensi array adalah jumlah indeks pada variabel array. Array multi dimensi (lebih dari satu indeks, maksimal 7 indeks). Dalam perhitungan, array sering digunakan untuk operasi matriks.
Matriks atau array dua dimensi adalah array yang memiliki dua atau lebih kolom dengan banyak baris, atau dua atau lebih baris dengan banyak kolom.

Soal:
1. Input banyaknya baris dan kolom lalu diisi nilai. setelah diisi nilai, tukar baris jadi kolom dan kolom jadi baris. 
2. Buat pada array 2 dimensi angka angka (baris dan kolom diinput). Setelah diinput angka angkanya, tampilkan bilangan yang bisa habis dibagi 3,5,7.


##Source Code

  #include <iostream>
  #include <iomanip> 
  using namespace std;
 
  int main()
  {
	int matriks[100][100];
  int baris, kolom, b, k;
  
	cout << "Nama : Yunisa Dwi Indrayani" <<endl;
	cout << "NIM  : 1227050135" <<endl;
	cout << "=======================================================" <<endl;
	cout << "Program Input Nilai Menggunakan Baris Dan Kolom" <<endl;
	cout << "=======================================================" <<endl;
	
 
  	cout << "Masukkan Jumlah Baris : ";
  	cin >> baris;
 
	cout << "Masukkan Jumlah Kolom : ";
	cin >> kolom;
	cout << endl;
 
  	// proses input 
  	for(b = 0; b < baris ; b++){
    	for(k = 0; k < kolom; k++){
		
		cout << "Baris " <<b+1<<", Kolom "<<k+1<< " = ";
      	cin >> matriks[b][k];
    }
    cout << endl;
    }
  
	cout << "=======================================================" <<endl;
 
  	cout << "Hasil matriks: " << endl;
 
  	// proses menampilkan array
  	for(b = 0; b < baris ; b++){
    	for(k = 0; k < kolom; k++){
	
	cout << setw(3) << matriks[b][k] << " ";
    }
    cout << endl;
    }
  
  	cout << "=======================================================" <<endl;
  
  	cout << "Hasil matriks setelah ditukar: " << endl;
  
  	//proses menukar baris dan kolom
  	for (b = 0; b < kolom; b++) {
  		for (k = 0; k < baris; k ++) {
  			cout << " " << matriks[k][b];
	   }
	  cout <<endl <<endl;
    }
  
  	cout << "===========================================================================" <<endl;
  	cout << "Program Menampilkan Bilangan Yang Habis dibagi 3,5,7 Pada Array 2 Dimensi" <<endl;
  	cout << "===========================================================================" <<endl;
  	
  	cout << "Bilangan Yang Habis Dibagi 3,5,7: "<<endl<<endl;
  	
  	// Menampilkan bilangan yang habis di bagi 3,5,7
	for (int b = 0; b < kolom; b++){
	for (int k = 0; k < baris; k++){
		if (matriks[b][k] % 3 == 0|| matriks [b][k] % 5 ==0||matriks [b][k] %7 ==0) cout << matriks[b][k] << ", ";
     }
    }

   return 0;
    }


##Output
Nama : Yunisa Dwi Indrayani
NIM  : 1227050135
=======================================================
Program Input Nilai Menggunakan Baris Dan Kolom
=======================================================
Masukkan Jumlah Baris : 2
Masukkan Jumlah Kolom : 3

Baris 1, Kolom 1 = 4
Baris 1, Kolom 2 = 5
Baris 1, Kolom 3 = 6

Baris 2, Kolom 1 = 6
Baris 2, Kolom 2 = 7
Baris 2, Kolom 3 = 8

-------------------------------------------------------
Hasil Matriks:
  4   5   6
  6   7   8
-------------------------------------------------------
Hasil Matriks Setelah Ditukar:
 4 6
 5 7
 6 8

===========================================================================
Program Menampilkan Bilangan Yang Habis dibagi 3,5,7 Pada Array 2 Dimensi
===========================================================================
Bilangan Yang Habis Dibagi 3,5,7:

5, 6, 7, 0, 0,
--------------------------------
Process exited after 30.51 seconds with return value 0
Press any key to continue . . .
