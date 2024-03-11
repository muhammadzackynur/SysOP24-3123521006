OPERATION AND FUNCTION OF OPERATING SYSTEM
Tujuan utama sistem operasi adalah untuk meningkatkan produktivitas sumber daya pemrosesan, seperti perangkat keras komputer atau pengguna sistem komputer. Kenyamanan dan produktivitas pengguna adalah pertimbangan sekunder. Di ujung lain spektrum, sebuah OS mungkin dirancang untuk pribadi komputer seharga beberapa ribu dolar dan melayani satu pengguna yang gajinya tinggi. Di dalam Dalam hal ini, penggunalah yang produktivitasnya ingin ditingkatkan sebanyak mungkin, dengan perangkat keras pemanfaatan menjadi kurang perhatian. Dalam sistem pengguna tunggal, penekanannya adalah pada pembuatan sistem komputer lebih mudah digunakan dengan menyediakan grafis dan mudah-mudahan lebih jelas secara intuitif antarmuka pengguna.

A.	Operations and funcations of OS
	The main operations and functions of an operating system are as follows: 
1. Process Management 
2. Memory Management 
3. Secondary Storage Management 
4. I/O Management
5. File Management
6. Protection 
7. Networking Management 
8. Command Interpretation. 
__________________________________________________________________________________
1.	Process Management 

CPU mengeksekusi sejumlah besar program. Sedangkan perhatian utamanya adalah eksekusi pengguna program, CPU juga diperlukan untuk aktivitas sistem lainnya. Kegiatan-kegiatan ini disebut proses.Proses adalah program yang sedang dieksekusi. Biasanya, pekerjaan batch adalah sebuah proses. Pengguna yang berbagi waktu program adalah sebuah proses. Tugas sistem, seperti spooling, juga merupakan sebuah proses. Untuk saat ini, suatu proses mungkin dianggap sebagai pekerjaan atau program berbagi waktu, namun konsepnya sebenarnya lebih umum

2.	Memory Management
Memori merupakan bagian termahal dalam sistem komputer. Memori adalah sejumlah besar kata atau byte, masing-masing dengan alamatnya sendiri. Interaksi dicapai melalui serangkaian pembacaan atau penulisan alamat memori tertentu. CPU mengambil dan menyimpannya di memori.
Ada berbagai algoritma yang bergantung pada situasi tertentu untuk mengelola memori. Pemilihan skema manajemen memori untuk sistem tertentu bergantung pada banyak faktor, namun terutama pada desain perangkat keras sistem. Setiap algoritma memerlukan perangkat kerasnya sendiri mendukung.

3.	Secondary Storage Management 

Tujuan utama sistem komputer adalah untuk menjalankan program. Program-program ini, bersama dengan data yang mereka akses, harus berada di memori utama selama eksekusi. Karena memori utama juga kecil untuk menampung semua data dan program secara permanen, sistem komputer harus menyediakannya penyimpanan sekunder untuk cadangan memori utama. Kebanyakan sistem komputer modern menggunakan disk sebagai penyimpanan informasi on-line utama, baik program maupun data. Sebagian besar program, seperti kompiler, perakit, rutinitas pengurutan, editor, pemformat, dan sebagainya, disimpan di disk hingga dimuat ke dalam memori, dan kemudian menggunakan disk sebagai sumber dan tujuan pemrosesannya. Oleh karena itu pengelolaan penyimpanan disk yang tepat sangat penting bagi sistem komputer.

4.	 I/O Management

Salah satu tujuan sistem operasi adalah untuk menyembunyikan kekhasan atau perangkat keras tertentu perangkat dari pengguna. Misalnya, di UNIX, kekhasan perangkat I/O disembunyikan dari sebagian besar sistem operasi itu sendiri oleh sistem I/O. Sistem operasi bertanggung jawab atas aktivitas berikut sehubungan dengan manajemen I/O:
1. Sistem cache buffer
2. Untuk mengaktifkan kode driver perangkat umum
3. Untuk menjalankan perangkat lunak driver untuk perangkat keras tertentu jika diperlukan.

5.	File Management

Manajemen file adalah salah satu layanan sistem operasi yang paling terlihat. Komputer dapat menyimpan informasi dalam beberapa bentuk fisik yang berbeda: pita magnetik, disk, dan drum adalah yang paling banyak bentuk umum. Masing-masing perangkat ini memiliki karakteristik dan organisasi fisiknya sendiri. Untuk kemudahan penggunaan sistem komputer, sistem operasi menyediakan tampilan logis yang seragam penyimpanan informasi. Sistem operasi mengabstraksi sifat fisik penyimpanannya perangkat untuk mendefinisikan unit penyimpanan logis, À le. File dipetakan, oleh sistem operasi, ke dalamnya perangkat fisik


6.	 Protection 

Perlindungan Berbagai proses dalam suatu sistem operasi harus dilindungi dari aktivitas satu sama lain. Untuk mencapai tujuan tersebut, berbagai mekanisme yang dapat digunakan untuk memastikan bahwa file, segmen memori, CPU dan sumber daya lainnya hanya dapat dioperasikan oleh proses-proses yang telah berfungsi dengan baik otorisasi dari sistem operasi.


7.	Networking Management 

Jaringan Sistem terdistribusi adalah kumpulan prosesor yang tidak berbagi memori atau jam. Sebaliknya, masing-masing prosesor memiliki memori lokalnya sendiri, dan prosesor berkomunikasi satu sama lain melalui berbagai jalur komunikasi, seperti bus berkecepatan tinggi atau saluran telepon. Sistem terdistribusi bervariasi dalam ukuran dan fungsi. Mereka mungkin melibatkan mikroprosesor, workstation, komputer mini, dan sistem komputer tujuan umum yang besar

8.	 Command Interpretation. 

Interpretasi Perintah Salah satu komponen terpenting dari sistem operasi adalah penerjemah perintahnya. Itu penerjemah perintah adalah antarmuka utama antara pengguna dan seluruh sistem. Banyak perintah yang diberikan kepada sistem operasi melalui pernyataan kontrol. Ketika pekerjaan baru dimulai dalam sistem batch atau ketika pengguna masuk ke sistem berbagi waktu, sebuah program akan membaca dan menafsirkan pernyataan kontrol dijalankan secara otomatis. Program ini disebut dengan berbagai cara (1) juru bahasa kartu kendali, (2) juru bahasa baris perintah, (3) shell (di Unix), dan seterusnya. Fungsinya cukup sederhana.

B. 	Jenis Sistem Operasi

Sistem operasi komputer modern dapat diklasifikasikan menjadi tiga kelompok, yang dibedakan
berdasarkan sifat interaksi yang terjadi antara pengguna komputer dan programnya
selama pemrosesannya. Ketiga kelompok tersebut disebut batch, time-sharing, dan real-time operating sistem.

C. 	Operating System: Examples

1.	Sistem Operasi Disk (DOS) 
DOS (Disk Operating System) adalah sistem operasi pertama yang banyak diinstal untuk personal komputer. Ini adalah program kontrol utama yang dijalankan secara otomatis saat Anda memulai program pribadi Anda komputer (PC). DOS tetap berada di komputer sepanjang waktu sehingga Anda dapat menjalankan program dan mengelolanya Itu. Ini adalah sistem operasi pengguna tunggal dari Microsoft untuk PC. Itu adalah OS pertama untuk PC dan merupakan program kontrol yang mendasari untuk Windows 3.1, 95, 98 dan ME. Windows NT, 2000 dan XP meniru DOS untuk mendukung aplikasi DOS yang ada

2.	UNIX
Sistem operasi UNIX digunakan pada produk workstation yang banyak dijual dari Sun Microsystems, Silicon Graphics, IBM, dan sejumlah perusahaan lainnya. Lingkungan UNIX dan model program klien/server merupakan elemen penting dalam pengembangan Internet dan pembentukan kembali komputasi yang berpusat pada jaringan dan bukan pada komputer individual. Linux, turunan UNIX yang tersedia dalam “perangkat lunak bebas” dan versi komersial, semakin meningkat popularitas sebagai alternatif untuk sistem operasi berpemilik.

	3 jendela
Windows adalah sistem operasi komputer pribadi dari Microsoft yang, bersama dengan beberapa lainnya Aplikasi bisnis yang umum digunakan seperti Microsoft Word dan Excel, sudah menjadi hal yang de facto “standar” untuk pengguna individu di sebagian besar perusahaan dan juga di sebagian besar rumah. Windows berisi jaringan internal, yang memungkinkan pengguna untuk berbagi file dan aplikasi satu sama lain jika mereka memilikinya PC terhubung ke jaringan. Di perusahaan besar, klien Windows sering kali terhubung ke a jaringan server UNIX dan NetWare. Versi server Windows NT dan 2000 semakin meningkat pangsa pasar, memberikan solusi khusus Windows untuk klien dan server. jendela adalah didukung oleh Microsoft, perusahaan perangkat lunak terbesar di dunia, serta Windows industri pada umumnya, yang mencakup puluhan ribu pengembang perangkat lunak.

D. 	Ringkasan

-	Sistem operasi dapat diklasifikasikan berdasarkan jumlah tugas yang dapat mereka lakukan “secara bersamaan” dan berapa banyak pengguna yang dapat menggunakan sistem “secara bersamaan”. Ituadalah: pengguna tunggal atau multi-pengguna dan tugas tunggal atau multi-tugas.
-	Sistem multi-pengguna jelas harus multi-tasking.
-	 Solusi yang mungkin untuk masalah fragmentasi eksternal adalah dengan mengizinkan alamat logis ruang suatu proses menjadi tidak bersebelahan, sehingga memungkinkan suatu proses dialokasikan secara fisik memori dimanapun yang terakhir tersedia.
-	 Memori fisik dipecah menjadi blok-blok berukuran tetap yang disebut frame. Memori logis juga dipecah menjadi blok-blok dengan ukuran yang sama yang disebut halaman.
-	 Perlindungan memori dalam lingkungan halaman dilakukan dengan bit perlindungan yang ada terkait dengan setiap frame.
-	Segmentasi adalah skema manajemen memori yang mendukung pandangan pengguna terhadap memori.
-	Segmentasi kemudian dapat menyebabkan fragmentasi eksternal, ketika semua blok memori bebas ada 3
terlalu kecil untuk menampung satu segmen
E. 	 KeyWords

Sistem berkerumun adalah sekelompok komputer yang digabungkan secara longgar dan bekerja bersamaerat sehingga dalam banyak hal mereka dapat dipandang seolah-olah mereka adalah satu komputer. Sistem Terdistribusi: Sistem terdistribusi adalah sistem komputer di mana sumber daya berada dalam unit-unit terpisah yang dihubungkan oleh suatu jaringan, tetapi menyajikan komputasi yang seragam kepada pengguna lingkungan

Sejarah OS

Introduction to Operating System
An Operating System (OS) is a collection of programs that acts as an interface between a user of a computer and the computer hardware. The purpose of an operating system is to provide an environment in which a user may execute the programs. Operating Systems are viewed as resource managers. The main resource is the computer hardware in the form of processors, storage, input/output devices, communication devices, and data. Some of the operating system functions are: implementing the user interface, sharing hardware among users, allowing users to share data among themselves, preventing users from interfering with one another, scheduling resources among users, facilitating input/output, recovering from errors, accounting for resource usage, facilitating parallel operations, organising data for secure and rapid access, and handling network communications

Operating System: Meaning
dimuat ke komputer oleh program boot, mengelola semua program lain di komputer. Program lainnya disebut aplikasi atau program aplikasi. Program aplikasimemanfaatkan sistem operasi dengan membuat permintaan layanan  melalui Aplikasi yang ditentukan Antarmuka Program (API). Selain itu, pengguna dapat berinteraksi langsung dengan sistem operasi melalui antarmuka pengguna seperti bahasa perintah atau Antarmuka Pengguna Grafis (GUI)

History of Computer Operating Systems
Komputer awal tidak memiliki sistem operasi apa pun. Pengguna hanya dapat menggunakan mesin dan akan tiba dengan membawa program dan data, seringkali dalam bentuk kertas dan selotip. Program akan dimuat ke dalam mesin, dan mesin akan diatur untuk bekerja hingga program selesai atau rusak. Program umumnya dapat di-debug melalui panel depan menggunakan sakelar dan lampu. Dikatakan bahwa Alan Turing adalah ahlinya pada mesin awal Manchester Mark I
