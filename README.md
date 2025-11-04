# TestUKLS3-1-
# Program Penjumlahan Dua Matriks

## 🧩 Deskripsi Singkat
Program **TestUKLS32 (PenjumlahanMatriks)** adalah program berbasis **Java** yang digunakan untuk melakukan **penjumlahan dua buah matriks berukuran sama**.  
Program ini meminta pengguna untuk memasukkan ukuran matriks (baris dan kolom), lalu mengisi elemen-elemen dari matriks A dan matriks B, kemudian menampilkan hasil penjumlahan dari kedua matriks tersebut.

---

## ⚙️ Cara Kerja Program

1. **Input Ukuran Matriks**
   ```java
   System.out.print("Masukkan jumlah baris matriks: ");
   int baris = input.nextInt();
   System.out.print("Masukkan jumlah kolom matriks: ");
   int kolom = input.nextInt();

-Pengguna menentukan jumlah baris dan kolom matriks (misal: 2x2 atau 3x3).

2. **Deklarasi Matriks**
int[][] matriksA = new int[baris][kolom];
int[][] matriksB = new int[baris][kolom];
int[][] hasil = new int[baris][kolom];

Matriks A, B, dan hasil penjumlahan disiapkan dalam bentuk array dua dimensi.

3. **Input Elemen Matriks A dan B**
   for (int i = 0; i < baris; i++) {
    for (int j = 0; j < kolom; j++) {
        System.out.print("A[" + i + "][" + j + "] = ");
        matriksA[i][j] = input.nextInt();
    }
}

-Pengguna mengisi elemen matriks satu per satu.
-Proses serupa dilakukan untuk matriks B.

4. **Penjumlahan Matrix**
   for (int i = 0; i < baris; i++) {
    for (int j = 0; j < kolom; j++) {
        hasil[i][j] = matriksA[i][j] + matriksB[i][j];
    }
}

-Setiap elemen dari matriks A dijumlahkan dengan elemen yang sesuai dari matriks B.
hasil[i][j]=A[i][j]+B[i][j]

5. **Menampilkan Hasil Penjumlahan**
   System.out.println("Hasil penjumlahan matriks A + B adalah:");
for (int i = 0; i < baris; i++) {
    for (int j = 0; j < kolom; j++) {
        System.out.print(hasil[i][j] + "\t");
    }
    System.out.println();
}

-Program menampilkan hasil penjumlahan dalam bentuk matriks yang rapi.

**🧮 Contoh Output**
Masukkan jumlah baris matriks: 2
Masukkan jumlah kolom matriks: 2
Masukkan elemen matriks A:
A[0][0] = 1
A[0][1] = 2
A[1][0] = 3
A[1][1] = 4
Masukkan elemen matriks B:
B[0][0] = 5
B[0][1] = 6
B[1][0] = 7
B[1][1] = 8

Hasil penjumlahan matriks A + B adalah:
6	8	
10	12	

**💡 Kesimpulan**
Program ini menunjukkan penerapan:
-Array dua dimensi di Java
-Perulangan bersarang (for dalam for)
-Operasi aritmetika elemen per elemen antar-matriks

Program ini dapat dikembangkan lebih lanjut dengan fitur tambahan seperti:
-Pengurangan dan perkalian matriks
-Validasi agar ukuran matriks harus sama
-Format tampilan hasil yang lebih rapi

**🖥️ Cara Menjalankan**

-Simpan kode dalam file: TestUKLS32.java
-Kompilasi program: javac TestUKLS32.java
-Jalankan program

<img width="515" height="231" alt="Screenshot 2025-11-04 163004" src="https://github.com/user-attachments/assets/bf3b1158-f186-49f6-b1ca-1167606bb5a7" />
