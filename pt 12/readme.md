-Dining Philosophers Problem

-Pengantar

  Masalah Dining Philosophers adalah salah satu masalah klasik dalam bidang pemrograman paralel dan komputasi konkuren. Diperkenalkan oleh Edsger Dijkstra pada tahun 1965, masalah ini      digunakan untuk menggambarkan dan mengatasi masalah yang muncul dalam pengelolaan sumber daya yang dibagi di antara beberapa proses.

#Deskripsi Masalah

  Bayangkan ada lima filsuf yang duduk mengelilingi meja bundar. Di antara setiap dua filsuf terdapat satu garpu, sehingga total ada lima garpu. Setiap filsuf menghabiskan hidupnya dengan bergantian berpikir dan makan. Untuk makan, seorang filsuf membutuhkan dua garpu: satu dari kiri dan satu dari kanan. Masalahnya adalah bagaimana memastikan bahwa tidak ada filsuf yang kelaparan (deadlock) atau tersendat (starvation).

Tantangan

  --Deadlock: Terjadi ketika setiap filsuf mengambil garpu di sebelah kiri pada waktu yang sama, sehingga tidak ada yang bisa mengambil garpu di sebelah kanan dan mulai makan.
  --Starvation: Terjadi ketika satu atau lebih filsuf tidak pernah mendapatkan kedua garpu yang diperlukan untuk makan, meskipun tidak ada deadlock.
    Solusi Potensial

1.Menggunakan Semaphore: Menggunakan semaphore untuk mengontrol akses ke garpu.

  -Setiap filsuf harus mengambil dua semaphore (satu untuk setiap garpu) sebelum mulai makan.
  -Melepaskan kedua semaphore setelah selesai makan.

2.Hierarchical Resource Allocation: Mengatur filsuf untuk mengambil garpu dalam urutan tertentu.

  -Misalnya, filsuf mengambil garpu kiri terlebih dahulu, kecuali filsuf terakhir yang mengambil garpu kanan terlebih dahulu untuk menghindari deadlock.

3.Resource Hierarchy Solution: Setiap garpu diberi nomor dan filsuf harus mengambil garpu dengan nomor lebih rendah terlebih dahulu.

  -Hal ini mencegah deadlock dengan memastikan urutan pengambilan garpu yang konsisten.

##Reader-Writer Problem

#Pengantar

Masalah Reader-Writer adalah masalah klasik dalam pengendalian konkuren yang berhubungan dengan sinkronisasi akses ke sumber daya bersama. Masalah ini sering muncul dalam database atau struktur data yang dibaca dan ditulis oleh banyak thread atau proses.

#Deskripsi Masalah

- Readers: Proses yang hanya membaca data.
- Writers: Proses yang dapat membaca dan menulis data.
 
#Tujuannya adalah untuk mengelola akses ke sumber daya sehingga:

- Beberapa pembaca bisa membaca data secara bersamaan tanpa saling mengganggu.
- Penulis harus memiliki akses eksklusif ke data, yang berarti tidak boleh ada pembaca atau penulis lain yang mengakses data saat seorang penulis sedang menulis.
  
#Tantangan

- Race Condition: Keadaan di mana hasil dari operasi tergantung pada urutan eksekusi yang tidak diinginkan.
- Deadlock: Ketika dua atau lebih proses menunggu satu sama lain untuk melepaskan sumber daya yang diinginkan.
- Starvation: Ketika satu atau lebih proses tidak pernah mendapatkan akses ke sumber daya yang dibutuhkan.
  
#Solusi Potensial

  1.Reader Preference Solution: Memberikan prioritas kepada pembaca.
      -Pembaca bisa terus membaca selama tidak ada penulis yang menunggu. Namun, ini bisa menyebabkan penulis mengalami starvation.
      
  2.Writer Preference Solution: Memberikan prioritas kepada penulis.
      -Jika seorang penulis ingin menulis, pembaca baru tidak diizinkan untuk memulai membaca sampai penulis selesai. Ini bisa menyebabkan pembaca mengalami starvation
  3.Fair Reader-Writer Solution: Menggunakan algoritma yang adil untuk memastikan tidak ada proses yang mengalami starvation.
      -Semaphore atau mekanisme sinkronisasi lain dapat digunakan untuk menjaga keseimbangan antara pembaca dan penulis, memastikan bahwa semua proses mendapatkan giliran yang adil untuk        mengakses sumber daya.
