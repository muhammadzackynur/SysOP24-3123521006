![Cuplikan layar 2024-03-25 192256](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/984966dd-77b1-436d-94a2-90424a183428)

 jadi cpu mengambil instruksi di alamat 0 di memori dan memasukkannya ke dalam register instruksi

![Cuplikan layar 2024-03-25 192352](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/16aa25d8-ea0d-4920-9fb3-467bcd2805df)

cpu menerjemahkan instruksi, bagian pertama adalah instruksi dan bagian kedua adalah lokasi dalam kasus kita instruksi dimuat dan alamatnya 6 jadi kita akan memuat nilai di alamat 6 ke dalam akumulator

![Cuplikan layar 2024-03-25 192519](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/7e9d4498-5ce5-45eb-80fc-9aad68d9bc29)

cpu menjalankan instruksi ini, mengambil nilai di alamat 6 dan memuatnya ke akumulator dalam hal ini nilainya adalah 1

![Cuplikan layar 2024-03-25 193041](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/2430ae38-422c-44c4-9f1c-29ff61200183)

penghitung program bertambah dan cpu mengambil instruksi berikutnya di bit berikutnya dalam memori

![Cuplikan layar 2024-03-25 193121](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/bf7043c2-604e-46ab-aeb1-1fc388aad202)

CPU menerjemahkan instruksi kali ini ADD dan alamatnya adalah 7 jadi kita akan menambahkan apa yang ada di alamat 7 ke dalam apa yang sudah ada di akumulator

![Cuplikan layar 2024-03-25 193202](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/e529827c-b870-4767-944e-6255acf057cd)

cpu mengeksekusi instruksi kita menambahkan nilai pada alamat 7 dalam hal ini nilai 1, 1+1=2

![Cuplikan layar 2024-03-25 193307](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/acbb4fcb-badc-4307-a6d7-5d40569d6f60)

dari lokasi memori berikutnya nomor 2

![Cuplikan layar 2024-03-25 193404](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/7c17cf6a-db64-4868-93f2-683a6510b278)

pada instruksi untuk menyimpan nilai dalam akumulator ke dalam ram, di alamat 6

![Cuplikan layar 2024-03-25 193525](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/a7b6c716-35f9-4bb5-992d-146ff9a0bcaa)

sekarang, perhatikan bahwa kita menimpa apa yang sudah ada sehingga alamat 6 sekarang memiliki 2 di dalamnya, bukan 1

![Cuplikan layar 2024-03-25 193623](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/86421678-b0a6-4f18-ba9e-54cbc76068a6)

instruksi berita lompat dengan lompat alamat berikutnya adalah yang ada di instruksi ini

![Cuplikan layar 2024-03-25 193728](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/cb9f9ead-feed-46eb-8ce8-455d90a7c665)

jadi akan melompat ke alamat nomor 1

![Cuplikan layar 2024-03-25 194441](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/ba4d3bea-dced-4321-87f3-5e504229da62)

penghitung program sekarang kembali ke 1 kemampuan untuk melompat, mengulang dan membuat instruksi secara rekursif adalah salah satu dasar ilmu komputer 

![Cuplikan layar 2024-03-25 194518](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/9b39ee23-ff8d-4b50-a3ba-b206086c69f5)

ambil dari lokasi 1

![Cuplikan layar 2024-03-25 194553](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/a53d7597-7f53-4edc-a207-6e65bb363914)

itu instruksi penambahan lagi

![Cuplikan layar 2024-03-25 200224](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/46990c58-9322-4a6c-ac35-a8323eada560)

program kita dengan instruksi sederhana ini, memang memiliki perintah halt atau cara apa pun untuk menghentikannya sehingga nilai tersebut akan terus bertambah satu hingga jumlahnya menjadi sangat besar sehingga tidak dapat lagi ditahan oleh alamat memori
