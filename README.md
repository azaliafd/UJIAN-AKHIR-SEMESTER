# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Azalia Fathimah Dinah
<br>NIM		:	1227050027
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 


## Deskripsi Umum
Array adalah kumpulan-kumpulan variabel yang menyimpan data dengan tipe yang sama atau data-data yang tersusun secara linear dimana di dalamnya terdapat elemen dengan tipe yang sama. Indeks dalam array menyatakan elemen yang disimpan dan panjang atau length menyatakan total elemen yang tersimpan. Elemen-elemen array biasanya ditulis dengan huruf besar disertai indeksnya yang berada di dalam kurung. Terdapat perbedaan mengenai cara penulisan indeks array antara bahasa C++ dan bahasa pemrograman lain.
Matriks adalah kumpulan bilangan atau simbol yang tertata rapi menurut baris dan kolom berbentuk segi empat. Bilangan-bilangan atau simbol-simbol yang terdapat dalam suatu matriks disebut dengan elemen-elemen matriks. Suatu matriks biasanya diberi nama dengan huruf kapital dan ditulis tebal. Elemen-elemen matriks biasanya diberi nama dengan huruf kecil yang sama dengan nama matriks tersebut, disertai 2 indeks bawah yang menunjukkan letaknya di dalam matriks. Indeks pertama menunjukkan baris sedangkan indeks kedua menunjukkan kolom. Jika salah satu dari baris dan kolom suatu matriks jumlahnya hanya satu maka elemen matriks tersebut hanya memiliki satu indeks. Matriks yang hanya memiliki satu indeks disebut dengan vektor.
Dalam bahasa pemrograman, suatu matriks direpresentasikan oleh array 2 dimensi sedangkan vektor direpresentasikan oleh array 1 dimensi.


## Source Code 1

    #include <iostream>
    using namespace std;
    int main() {
    /*1. A. Input banyaknya baris dan kolom array dimensi 2
    B. Isi dengan nilai
    C. Setelah nilai diisi, ubah baris menjadi kolom, dan kolom menjadi baris*/
    int nilai[100][100];
    int jum_baris, jum_kolom, a, z;
    cout << “Masukkan jumlah baris yang diinginkan : “;
    cin >> jum_baris;
    cout << “Masukkan jumlah kolom yang diinginkan : “;
    cin >> jum_kolom;
    cout << endl;
    for (a = 0; a < jum_baris ; a++){
    for (z = 0; z < jum_kolom; z++){
    cout << “Baris ke-” << a+1 << “, kolom ke-” << z+1 << “ = “;
    cin >> nilai[a][z];
    }
    cout << endl;
    }
    cout << “Hasil input : “ << endl << endl;
    for (a = 0; a < jum_baris ; a++){
    for (z = 0; z < jum_kolom; z++){
    cout << “ “<< nilai[a][z] << “ “;
    }
    cout << endl;
    }
    cout << “=============================================” << endl << endl;
    for (a = 0; a < jum_kolom ; a++){
    for (z = 0; z < jum_baris; z++){
    cout << “ “<< nilai[z][a] << “ “;
    }
    cout << endl;
    }
    }

## Output 1

![UAS DASPROG_AZALIA FD_1](https://user-images.githubusercontent.com/121106799/209097922-9f814bea-5c93-48e5-83e9-e26d280f8130.jpeg)


## Source Code 2

        #include <iostream>
        using namespace std;
        int main (){
        /*2. A. Deret matematika bilangan yang tidak habis dibagi 3, 5, dan 7.
        B. Inputnya, baris pertama merupakan banyaknya baris (bisa diinput 0–20)
        C. Baris kedua merupakan banyaknya kolom
        D. Outputnya, tampilnya bilangan yang tidak habis dibagi 3, 5 , dan 7*/
        int nilai [20][20];
        int jum_baris, jum_kolom, a, z;
        cout << “Masukkan jumlah baris yang diinginkan: “;
        cin >> jum_baris;
        cout << “Masukkan jumlah kolom yang diinginkan : “;
        cin >> jum_kolom;
        for (a = 0; a < jum_baris ; a++){
        for (z = 0; z < jum_kolom; z++){
        cout << “Baris ke-” << a+1 << “, kolom ke-” << z+1 << “ = “;
        cin >> nilai[a][z];
        }
        cout << endl;
        }
        cout << “Nilai yang diinputkan : \n”;
        for (int a = 0; a < jum_baris; a++){
        for (int z = 0; z < jum_kolom; z++){
        cout << nilai[a][z] << ”\t”;
        }
        cout << endl;
        }
        int angka[20];
        int indeks = 0;
        for (a = 0; a < jum_baris; a++){
        for (z = 0; z < jum_kolom; z++) {
        if (nilai[a][z] % 3 != 0 && nilai[a][z] % 5 != 0 && nilai[a][z] % 7 != 0){
        angka[indeks] = nilai[a][z];
        indeks++;
        }
        }
        }
        cout << “\nBilangan yang tidak bisa dibagi oleh bilangan 3, 5, 7 adalah “;
        for(int a = 0; a < indeks; a++){
        cout << angka[a] << “, “;
        }
        }

## Output 2

![UAS DASPROG_AZALIA FD_2](https://user-images.githubusercontent.com/121106799/209098332-88507613-e9db-4446-baab-bb57ed8c967a.jpeg)
