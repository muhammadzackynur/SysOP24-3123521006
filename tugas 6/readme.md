/NO 1. 

             Proses Eksikusi Program dalam Siklus CPU
- Siklus CPU
  * CPU mengambil instruksi dari memori utama (RAM) sesuai dengan alamat yang ditunjuk oleh Program Counter (PC).
  * Instruksi ini kemudian dimuat ke dalam register di dalam CPU untuk
-  Siklus CPU
  *  Setelah instruksi diambil, CPU mendekode instruksi tersebut untuk memahami operasi apa yang perlu dilakukan.
  * CPU mengidentifikasi opcode (kode operasi) dan operand (data yang diperlukan untuk operasi tersebut).
 -  Siklus CPU
  * Setelah instruksi didekode, CPU menjalankan instruksi tersebut.
  * melibatkan melakukan operasi aritmatika, logika, transfer data, atau instruksi kontrol lainnya.
 - Bahasa Pemrograman
  * Bahasa pemrograman memungkinkan programmer untuk menulis kode yang bisa dimengerti oleh manusia.
  * Bahasa pemrograman menyediakan struktur, sintaksis, dan aturan untuk menulis program.
 - Peran Compiler
  * Compiler menerjemahkan kode yang ditulis dalam bahasa pemrograman ke dalam bahasa mesin yang dapat dimengerti olehn 
     komputer.
  * Proses ini melibatkan kompilasi, optimasi, dan pembuatan output dalam bentuk file biner atau kode yang dapat dieksekusi.
 -  Peran Sistem Operasi
  * Sistem operasi bertanggung jawab atas manajemen sumber daya komputer, termasuk memori, CPU, perangkat 
    masukan/keluaran, dan penggunaan jaringan.
  * Sistem operasi menyediakan antarmuka antara perangkat keras dan perangkat lunak, serta mengelola proses, memori, dan 
    penggunaan CPU.

NO. 3
$ make 

![Cuplikan layar 2024-03-19 013913](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/e5145ec3-2e62-446c-b53b-c63c7b688944)

 perintah yang digunakan dalam lingkungan pengembangan perangkat lunak untuk mengotomatiskan proses kompilasi dan pembangunan proyek perangkat lunak. 

 $ make clean

![Cuplikan layar 2024-03-19 014019](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/adeb8a80-37be-4e02-a3aa-97440ce5bab6)

 dapat dengan cepat membersihkan proyek mereka dari file-file sementara dan file-file yang dihasilkan selama proses pembangunan

$ sudo make install 

![Cuplikan layar 2024-03-19 014120](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/16be61ff-a499-4348-b137-906bc39b19fe)

 perintah yang digunakan dalam lingkungan pengembangan perangkat lunak untuk menginstal perangkat lunak yang telah dikompilasi ke dalam sistem secara sistematis

$ iops64 $(nproc)
$ flops64 $(nproc)

![Cuplikan layar 2024-03-19 015511](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/28e8c415-a8d3-4a57-8f42-fcc972218ea7)

![Cuplikan layar 2024-03-19 020539](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/7dc207b8-abfd-4ddb-a5b0-eccd24fe4813)

$ iops32 $(nproc): Perintah ini digunakan untuk mengukur jumlah operasi integer per detik (IOPS) pada sistem dengan panjang bilangan bulat 32 bit. Ekspresi $(nproc) digunakan untuk mengambil jumlah CPU atau prosesor yang tersedia pada sistem, dan perintah $ iops32 mungkin akan menjalankan serangkaian operasi integer pada setiap prosesor, kemudian mengukur dan melaporkan jumlah operasi per detik yang berhasil dilakukan.

$ iops64 $(nproc): Sama seperti perintah sebelumnya, namun untuk operasi integer 64 bit.

$ flops32 $(nproc): Perintah ini mungkin digunakan untuk mengukur jumlah operasi floating-point per detik (FLOPS) pada sistem dengan panjang bilangan pecahan 32 bit. 

$ flops64 $(nproc): Sama seperti perintah sebelumnya, namun untuk operasi floating-point 64 bit.
