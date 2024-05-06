# Percobaan 1 : File descriptor
- $ ps
  
![Cuplikan layar 2024-03-18 211042](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/bab243af-8ab8-4e72-b93f-cd011974d8e9)

 menampilkan daftar proses yang sedang berjalan di sistem

- $ cat
  
 hallo, apa khabar
 hallo, apa khabar
 exit dengan ^d
 exit dengan ^d
 [Ctrl-d]
 
![Cuplikan layar 2024-03-18 211059](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/979def4d-843b-4c4c-b3cf-c672542040ab)

menampilkan isi file atau teks yang dimasukkan langsung dari terminal

- $ mkdir mydir
  $ mkdir mydir **(Terdapat pesan error)**
  
![Cuplikan layar 2024-03-18 211500](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/02266554-f12d-4702-90ba-28217f901e0a)

 digunakan untuk membuat direktori baru di sistem file

## Percobaan 2 : Pembelokan (redirection)

-  $ cat 1> myfile.txt
  
 Ini adalah teks yang saya simpan ke file myfile.txt
 
![Cuplikan layar 2024-03-18 213014](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/b38e3404-60c2-49cb-91ac-5218e447f367)

 menyalin teks yang dimasukkan melalui terminal ke dalam file yang ditentukan

-  $ cat 0< myfile.txt
   $ cat myfile.txt

![Cuplikan layar 2024-03-18 213041](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/66749eaf-898e-4149-8242-b78438f9fe92)

 menggunakan operator redirection < untuk mengarahkan input dari file yang disebut 
 
 myfile.txt ke perintah cat

-  $ mkdir
   $mydir (Terdapat pesan error)
   $ mkdir mydir 2> myerror.txt
   $ cat myerror.txt

![Cuplikan layar 2024-03-18 213155](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/dcb1fa4e-ba9b-472f-be12-886b1c8d1b8b)

-perintah mkdir, dapat mengarahkan keluaran kesalahan (stderr) ke file menggunakan 
 operator 2> seperti yang Anda lakukan sebelumnya
-membuat direktori "mydir" dan mengalirkan pesan kesalahan ke dalam file myerror.txt
-menampilkan pesan kesalahan yang dihasilkan oleh perintah mkdir, jika ada, atau akan 
 menampilkan pesan kosong jika tidak ada kesalahan yang terjadi

-  $ ls filebaru (Terdapat pesan error)
   $ ls filebaru 2> out.txt
   $ cat out.txt
   $ ls filebaru 2> out.txt 2>&
   $ cat out.txt

![Cuplikan layar 2024-03-18 213459](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/b13f3b11-eaf3-4d22-a57d-b1a828ac62fb)
   
    $ ls filebaru: Ini mencoba untuk menampilkan isi dari direktori atau file dengan nama "filebaru". Jika tidak ada file atau direktori dengan nama tersebut, maka akan muncul pesan kesalahan.

    $ ls filebaru 2> out.txt: Ini menjalankan perintah yang sama dengan langkah pertama, tetapi pesan kesalahan dialirkan ke dalam file out.txt menggunakan operator redirection 2>. Jika tidak ada kesalahan, file out.txt akan tetap kosong.

    $ cat out.txt: Ini mencetak isi dari file out.txt. Jika tidak ada pesan kesalahan yang dihasilkan pada langkah kedua, maka file out.txt akan tetap kosong dan tidak akan ada output yang ditampilkan.

    $ ls filebaru 2> out.txt 2>&: Pada langkah ini, terjadi kesalahan dalam sintaks. Pada bagian akhir perintah, 2>& tidak diikuti oleh nomor file descriptor atau alamat file yang valid. Ini akan menyebabkan kesalahan sintaks pada shell.

    $ cat out.txt: Karena langkah keempat menghasilkan kesalahan sintaks, perintah ini tidak dijalankan. Oleh karena itu, tidak ada perubahan pada file out.txt, dan file tersebut akan tetap kosong.

- $ echo “mencoba menulis file” 1> baru
  $ cat filebaru 2> baru 1>&
  $ cat baru

![Cuplikan layar 2024-03-18 213756](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/54f1856c-e33d-4fa3-aa65-de42215aaeff)

 menampilkan isi dari file "filebaru", kemudian akan mengalirkan pesan kesalahan ke file "baru" dan output standar (stdout) ke file yang sama, yaitu "baru".

- $ echo “kata pertama” > surat
  $ echo “kata kedua” >> surat
  $ echo “kata ketiga” >> surat
  $ cat surat
  $ echo “kata keempat” > surat
  $ cat surat

![Cuplikan layar 2024-03-18 214107](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/96ce8c49-305c-4219-b73b-82ab756b41c4)

 ''$ cat surat'' akan menampilkan hanya "kata keempat" karena langkah sebelumnya telah 
   menggantikan isi file "surat" yang sebelumnya

- $ cat <<++
  Hallo, apa kabar?
  Baik-baik saja?
  Ok!
  ++
  $ cat <<%%%
  Hallo, apa kabar?
  Baik-baik saja?
  Ok!
  %%%

![Cuplikan layar 2024-03-18 214214](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/9a6ce010-6393-438e-badc-711bb69e4d65)

- $ cat myfile.txt – surat

![Cuplikan layar 2024-03-18 214250](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/680b9531-cdb1-46bf-bc08-caa8292131bc)

Perintah tersebut akan menggabungkan isi dari kedua file tersebut dan menampilkan hasilnya di layar terminal

## Percobaan 3 : Pipa (pipeline)

- $ who
  $ who | sort
  $ who | sort –r
  $ who > tmp
  $ sort tmp
  $ rm tmp
  $ ls –l /etc | more
  $ ls –l /etc | sort | more

![Cuplikan layar 2024-03-18 214545](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/6328d21b-88f5-446c-a91c-2ab29b04e508)

![Cuplikan layar 2024-03-18 214601](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/4a800e97-2e9f-4bde-8345-4867465419ac)

   $ who: Perintah ini menampilkan daftar pengguna yang saat ini masuk (login) ke sistem.
   $ who | sort: Perintah ini mengalirkan output dari perintah who ke perintah sort, yang 
     kemudian akan mengurutkan daftar pengguna berdasarkan urutan abjad (nama 
     pengguna).
  $ who | sort -r: Perintah ini seharusnya mengurutkan daftar pengguna dalam urutan 
     terbalik, tetapi ada kesalahan penulisan. Simbol -r digunakan untuk memberitahu sort 
     agar mengurutkan secara terbalik (descending order).
 $ who > tmp: Perintah ini menyimpan output dari perintah who ke dalam file sementara 
    bernama "tmp".
 $ sort tmp: Perintah ini mengurutkan isi file sementara "tmp" secara default (ascending 
    order).
 $ rm tmp: Perintah ini menghapus file sementara "tmp" yang telah dibuat sebelumnya.
 $ ls -l /etc | more: Perintah ini menampilkan daftar isi dari direktori /etc secara rinci (long 
    listing format) dan kemudian mengalirkan outputnya ke perintah more, yang 
    memungkinkan Anda melihat output satu halaman sekaligus.
 $ ls -l /etc | sort | more: Perintah ini menampilkan daftar isi dari direktori /etc, kemudian 
    mengurutkannya, dan akhirnya menampilkannya dengan menggunakan perintah more. 
    Ini memastikan bahwa daftar isi yang ditampilkan sudah diurutkan sebelum Anda 
    melihatnya halaman per halaman.

- $ echo hello
  $ echo hello > output
  $ cat output

![Cuplikan layar 2024-03-18 214728](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/2bdbd3e7-6164-47d9-a865-9027d35fd974)

$ echo hello: Ini mencetak kata "hello" ke layar, tetapi tidak mengarahkan outputnya ke 
    mana pun, sehingga hanya akan ditampilkan di terminal.
 $ echo hello > output: Ini mencetak kata "hello" ke dalam file yang disebut "output". 
    Operator > digunakan untuk mengarahkan output dari perintah echo ke file "output". 
    Jika file "output" sudah ada, isi sebelumnya akan ditimpa dengan "hello". Jika tidak, file 
    "output" akan dibuat dan isinya akan menjadi "hello".
$ cat output: Ini menampilkan isi dari file "output" menggunakan perintah cat. Karena 
   perintah sebelumnya telah menulis "hello" ke dalam file "output", perintah ini akan 
   menampilkan "hello" di layar.

- $ echo bye >> output
  $ cat output

![Cuplikan layar 2024-03-18 214803](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/8c25b2df-5a44-4ed5-a5ec-f32ab107fa6e)

  $ echo bye >> output: Ini menambahkan kata "bye" ke dalam file yang sudah ada, yaitu 
    "output". Operator >> digunakan untuk menambahkan output dari perintah echo ke 
     akhir file "output".

  $ cat output: Ini menampilkan isi dari file "output" menggunakan perintah cat. Sekarang, 
     file "output" berisi dua baris teks: "hello" dan "bye".

- $ cat < output

![Cuplikan layar 2024-03-18 214843](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/391ea757-c087-4ce4-9a37-d97d9690f3b7)


- $ cat < output > out
  $ cat out
  $ cat < output >> out
  $ cat out
  $ cat < output > output
  $ cat output
  $ cat < out >> out (Proses tidak berhenti)
     [Ctrl-c]
  $ cat out

![Cuplikan layar 2024-03-18 215010](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/27152c84-144f-4d40-a385-55e90dac2d13)

    $ cat < output > out: Perintah ini membaca isi dari file "output" dan menyalinnya ke file "out". Ini dilakukan dengan menggunakan operator redirection < untuk membaca dari "output" dan > untuk menulis ke "out".

    $ cat out: Perintah ini menampilkan isi dari file "out". Isinya akan sama dengan isi dari file "output" karena langkah sebelumnya menyalinnya ke "out".

    $ cat < output >> out: Perintah ini membaca isi dari file "output" dan menambahkannya ke akhir file "out". Ini dilakukan dengan menggunakan operator redirection < untuk membaca dari "output" dan >> untuk menambahkan ke "out".

    $ cat out: Perintah ini menampilkan isi dari file "out". Sekarang, isi "out" akan terduplikasi karena langkah sebelumnya menambahkan isi "output" ke dalamnya.

    $ cat < output > output: Perintah ini mencoba menyalin isi dari file "output" ke dalam file "output" sendiri. Ini seharusnya tidak dilakukan karena bisa menyebabkan hasil yang tidak terdefinisi atau potensial kehilangan data.

    $ cat output: Perintah ini menampilkan isi dari file "output". Karena perintah sebelumnya tidak seharusnya mengubah isi "output", isinya tetap sama seperti sebelumnya.

    $ cat < out >> out: Perintah ini mencoba membaca isi dari file "out" dan menambahkannya ke akhir file "out". Namun, ada masalah dengan sintaks perintah ini, sehingga perintah tersebut tidak selesai dan tidak memberikan output yang diharapkan. Untuk menghentikan proses, Anda menggunakan Ctrl+C.

    $ cat out: Setelah membatalkan perintah sebelumnya dengan Ctrl+C, Anda mencoba menampilkan isi dari file "out" lagi. Karena perintah sebelumnya tidak berhasil menambahkan isi "out" ke akhirnya sendiri, isi "out" sebelumnya akan tetap sama.

## Percobaan 4 : Filter

-  $ w –h | grep <user>
   $ grep <user> /etc/passwd
   $ ls /etc | wc
   $ ls /etc | wc –l
   $ cat > kelas1.txt
   Badu
   Zulkifli
   Yulizir
   Yudi
   Ade
   [Ctrl-d]
   $ cat > kelas2.txt
   Budi
   Gama
   Asep
   Muchlis
 [Ctrl-d]
 $ cat kelas1.txt kelas2.txt | sort
 $ cat kelas1.txt kelas2.txt > kelas.txt
 $ cat kelas.txt | sort | uniq

![Cuplikan layar 2024-03-18 215444](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/ff2708f7-3e50-4ec0-aa60-2f976ae8ff8d)

![Cuplikan layar 2024-03-18 215458](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/e6d4d01a-3da6-400c-a380-16a6a437af66)

$ w -h | grep <user>: Perintah ini mencoba untuk menampilkan informasi tentang pengguna yang sedang login (tanpa header) menggunakan perintah w, kemudian menggunakan grep untuk mencari baris yang mengandung kata <user>. Namun, Anda harus mengganti <user> dengan nama pengguna yang ingin Anda cari, misalnya: $ w -h | grep myusername.

$ grep <user> /etc/passwd: Perintah ini mencari baris yang mengandung kata <user> dalam file /etc/passwd. Sama seperti sebelumnya, Anda perlu mengganti <user> dengan nama pengguna yang ingin Anda cari.

$ ls /etc | wc: Perintah ini mencetak jumlah baris, kata, dan byte dari output ls /etc, yang berisi daftar isi dari direktori /etc.

$ ls /etc | wc -l: Perintah ini menghitung jumlah baris dari output ls /etc, yang merupakan jumlah entri dalam direktori /etc.

$ cat > kelas1.txt: Perintah ini membuka editor teks untuk membuat atau mengedit file dengan nama kelas1.txt. Anda akan dapat mengetikkan teks secara interaktif, dan teks yang Anda masukkan akan disimpan dalam file tersebut


1. Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke 
   file baru.
   

![Cuplikan layar 2024-03-18 221711](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/21ccf117-4669-4776-8597-7183d139e45f)

 daftar lengkap dari isi direktori aktif akan disimpan dalam file baru

2. Lihat daftar secara lengkap pada direktori /etc/passwd, belokkan tampilan standard 
    output ke file baru tanpa menghapus file baru sebelumnya.
   

![Cuplikan layar 2024-03-18 221755](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/c2d8b196-0667-4b5f-aca8-3c4428d1b6ca)

3. Urutkan file baru dengan cara membelokkan standard input.
    
![Cuplikan layar 2024-03-18 221846](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/c3aa3fc4-7024-47ab-937e-00b4077d5f92)

4. Urutkan file baru dengan cara membelokkan standard input dan standard output ke file 
    baru.urut.
    
![Cuplikan layar 2024-03-18 221944](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/2dbefc06-0356-4ed5-a8e8-2183955fed76)

5. Buatlah direktori latihan 2 sebanyak 2 kali dan belokkan standard error ke file 
    rmdirerror.txt

![Cuplikan layar 2024-03-18 222114](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/5054ad84-9476-466b-9dfb-80e8c63955d0)

6. Urutkan kalimat berikut : 
           Jakarta
           Bandung
           Surabaya
           Padang
           Palembang
           Lampung
    Dengan menggunakan notasi here document (<@@@ ...@@@) . [HINT] 
    https://www.geeksforgeeks.org/how-to-use-here-document-in-bash-programming/)

![Cuplikan layar 2024-03-18 222318](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/cc799372-18f9-4baf-928d-16e7fd5cd5f9)

7. Hitung jumlah baris, kata dan karakter dari file baru.urut dengan menggunakan filter 
    dan tambahkan data tersebut ke file baru.

![Cuplikan layar 2024-03-18 222501](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/16e75d41-6f25-466b-9bf6-7aecda234c25)

8. Gunakan perintah di bawah ini dan perhatikan hasilnya. 

![Cuplikan layar 2024-03-18 222823](https://github.com/muhammadzackynur/SysOP24-3123521006/assets/160557480/ab90a0f2-342f-40b2-8686-a0f82371e986)

## KESIMPULAN : praktikum input dan output pada Debian memberikan pemahaman yang mendalam tentang bagaimana sistem operasi Linux mengelola masukan dan keluaran, serta keterampilan praktis yang sangat berguna bagi pengembang perangkat lunak dan administrator sistem.





