**CISC (Complex Instruction Set Computing):**

-  Didesain untuk mengeksekusi perintah yang kompleks dan bervariasi dalam satu siklus clock.
-  Memiliki set instruksi yang lebih kompleks dan beragam, termasuk instruksi yang melibatkan operasi matematika kompleks, manipulasi  string, dan akses memori yang kompleks.
-  Mengizinkan instruksi tunggal untuk melakukan tugas yang lebih rumit, sehingga dapat mengurangi jumlah instruksi yang diperlukan untuk menyelesaikan suatu program.
- 
**Contoh arsitektur CISC termasuk x86 (Intel dan AMD).**


**RISC (Reduced Instruction Set Computing):**

-  Didesain untuk mengeksekusi serangkaian instruksi yang sederhana dalam satu siklus clock.
-  Memiliki set instruksi yang relatif sederhana dan seragam, biasanya hanya mendukung operasi dasar seperti bekerja dengan bilangan bulat, manipulasi bit, dan transfer data.
-  Menekankan eksekusi instruksi dalam jumlah minimum tetapi dengan kecepatan tinggi.
-  Biasanya memerlukan beberapa instruksi untuk menyelesaikan tugas yang kompleks, tetapi setiap instruksi dapat dieksekusi dengan sangat cepat.

**Contoh arsitektur RISC termasuk ARM dan MIPS.**

![Difference-Between-CISC-And-RISC](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/b3aebbc4-7197-449a-af91-813f85d09476)

Perbedaan utama antara keduanya adalah kompleksitas instruksi dan pendekatan dalam mengeksekusi instruksi. CISC cenderung memiliki instruksi yang lebih kompleks tetapi dapat melakukan lebih banyak tugas dalam satu instruksi, sementara RISC memiliki instruksi yang lebih sederhana tetapi menekankan pada eksekusi yang lebih cepat.

**tugas Fork : Parent - Child Proses**

Akses dan clonning repo : https://github.com/ferryastika/operatingsystem.git Deskripsikan dan visualisasikan pohon proses hasil eksekusi dari kode program fork01.c, fork02.c, fork03.c.

![Cuplikan layar 2024-04-30 005251](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/5f77d8a7-dffc-48bc-bdd1-01a6b6c6961b)

**git clone https://github.com/ferryastika/operatingsystem.git**

![Cuplikan layar 2024-04-30 010756](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/ee37cf35-aeb8-4e44-a706-6d5d2659df1a)

**ls**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/99f17934-cc7f-4ec7-992d-b198053f7b67)

**cd operatingsystem**

**ls**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/23d51ae2-c76a-43c6-addf-6cc9fc32f47d)

**sudo -i**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/48709bfe-19a0-404b-a348-77732412d357)

Untuk menjalankan fork01.cpp menggunakan perintah g++ fork01.cpp -o fork01.exe

![Cuplikan layar 2024-04-30 011515](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/1ccf79bd-8813-4af3-bd47-0f49f36e0dde)

**Untuk menampilkan program menggunakan perintah nano fork01.cpp**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/654f65f7-eeba-45f2-8850-e3d21667bb02)

** ./fork01.exe**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/792867b8-5e66-4a33-b1e1-6f0533643f4b)

**fKemudian untuk menjalankan fork02.cpp dan juga fork03.cpp caranya sama seperti menjalankan fork01.cpp.**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/248d5827-8f5a-4afd-9676-f536ab3aac94)

**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/860d629e-af37-44d8-a96a-df26b1382504)

**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/b8f8cf77-9947-4a11-9aa3-2d3cc9571277)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/02e4e963-4614-44a4-980f-c461f7cbef31)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/d2894df4-b591-4227-abae-ebcdfcf9b716)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/2ae81c71-700d-43ea-8dd8-7aeb26a44e33)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/4e99a08e-4e49-46be-8796-1e344e6869f2)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/d7943b36-4265-4547-9838-bea4687a9bb3)

**./orphan.exe**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/5745b872-a26a-48c4-9f44-ea2a202168b0)

**child process**

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/d9f64a1a-4c1a-48f9-9063-0cef01f98020)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/657ba4c9-8fff-4836-90df-be0745cb09e1)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/13d1a472-7f2c-4eed-aee9-30534f35b35a)

- Perintah g++ zombie.c -o zombie.exe digunakan untuk mengkompilasi program C yang disimpan dalam file zombie.c menggunakan kompiler GNU C++ (g++). Opsi -o digunakan untuk menentukan nama file dari hasil kompilasi yang dihasilkan, dalam hal ini zombie.exe.

- Perintah nano zombie.c digunakan untuk membuka atau membuat file teks bernama zombie.c menggunakan editor teks Nano

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/b839da02-d404-413a-9cb9-57964ea6b891)

![image](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/79b8fd97-196b-417f-a441-ec6fddf79af7)











