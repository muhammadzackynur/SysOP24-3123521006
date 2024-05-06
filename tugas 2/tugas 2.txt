NAMA : MUHAMMAD ZACKY NUR S
NRP    : 3123521006

-Mindmap Sejarah dan Fungsi Os
-Perbedaan BIOS dan UEFI





##UEFI (Unified Extensible Firmware Interface) adalah sebuah antarmuka perangkat lunak yang menggantikan BIOS (Basic Input/Output System) tradisional dalam banyak komputer modern, terutama yang dibuat setelah tahun 2010. UEFI dirancang untuk memberikan antarmuka standar yang lebih canggih dan fleksibel antara sistem operasi dan perangkat keras komputer.

Berikut adalah beberapa poin penting tentang UEFI:

Fleksibilitas: UEFI dirancang untuk menjadi lebih fleksibel daripada BIOS tradisional. Ini memungkinkan pengembang perangkat keras untuk menyediakan lebih banyak fitur dalam BIOS komputer, seperti antarmuka grafis, dukungan perangkat penyimpanan besar, dan kemampuan boot yang lebih kuat.

Dukungan untuk HDD besar: UEFI mendukung partisi boot yang lebih besar daripada BIOS tradisional, yang memungkinkan penggunaan disk dengan kapasitas lebih besar dari 2 TB. Ini memungkinkan sistem operasi dan data yang lebih besar disimpan tanpa memerlukan partisi khusus.

Keamanan: UEFI menyertakan fitur keamanan yang lebih baik daripada BIOS, termasuk Secure Boot. Secure Boot memverifikasi integritas sistem boot sebelum memulai, mencegah sistem boot dari perangkat lunak yang tidak sah atau berbahaya.

Antarmuka Standar: UEFI menyediakan antarmuka standar yang dapat digunakan oleh berbagai sistem operasi. Ini memungkinkan pengembang sistem operasi untuk membuat perangkat lunak yang kompatibel dengan berbagai macam perangkat keras tanpa harus menyesuaikan dengan implementasi BIOS yang berbeda-beda.

EFI Partisi Sistem: UEFI menggunakan partisi EFI (Extensible Firmware Interface) sebagai partisi sistem boot, berbeda dengan BIOS yang menggunakan MBR (Master Boot Record). Partisi EFI menyediakan ruang yang terpisah untuk menyimpan file boot dan konfigurasi sistem, memisahkan data ini dari partisi data lainnya.



##BIOS (Basic Input/Output System) adalah perangkat lunak yang disematkan pada chip ROM (Read-Only Memory) di motherboard komputer. BIOS bertanggung jawab untuk menginisialisasi dan mengontrol perangkat keras dasar saat sistem komputer dihidupkan. Berikut beberapa poin penting tentang BIOS:

Inisialisasi Perangkat Keras: Saat komputer dinyalakan, BIOS memulai proses inisialisasi perangkat keras dasar seperti prosesor, RAM, kartu grafis, dan perangkat penyimpanan. Ini memastikan bahwa semua perangkat keras yang penting berfungsi dengan benar sebelum sistem operasi dimuat.

Bootloader: Setelah inisialisasi perangkat keras selesai, BIOS mencari dan memuat bootloader dari perangkat penyimpanan yang diprioritaskan (biasanya hard disk atau SSD). Bootloader adalah bagian kecil dari perangkat lunak yang bertanggung jawab untuk memuat sistem operasi ke dalam memori.

Konfigurasi Sistem: BIOS menyediakan antarmuka sederhana yang memungkinkan pengguna untuk mengonfigurasi berbagai pengaturan sistem, seperti urutan boot, pengaturan keamanan, pengaturan CPU, dan banyak lagi. Pengguna biasanya dapat mengakses layar konfigurasi BIOS dengan menekan tombol khusus saat komputer dinyalakan, seperti Del, F2, atau Esc.

Antarmuka Dasar: BIOS menyediakan antarmuka yang sederhana dan tidak tergantung pada sistem operasi yang diinstal. Ini memungkinkan BIOS untuk beroperasi secara independen dari sistem operasi yang ada di komputer.

Tingkat Rendah: BIOS bekerja pada tingkat rendah dan berfungsi bahkan sebelum sistem operasi dimuat. Ini membuatnya sangat penting untuk proses booting komputer dan inisialisasi perangkat keras awal.





##Perbedaan utama antara UEFI (Unified Extensible Firmware Interface) dan BIOS (Basic Input/Output System) terletak pada arsitektur, fitur, dan kemampuan masing-masing. Berikut adalah perbedaan antara keduanya:

Arsitektur:

BIOS: BIOS menggunakan arsitektur monolitik, yang berarti semua kode BIOS berada dalam satu blok besar yang sulit dimodifikasi atau diperluas.
UEFI: UEFI menggunakan arsitektur modular yang memungkinkan pengembang untuk menambahkan dan memperluas fungsionalitas dengan mudah. UEFI terdiri dari beberapa komponen yang saling terhubung dan dapat diperbarui secara independen.
Antarmuka Pengguna:

BIOS: BIOS memiliki antarmuka pengguna yang sederhana, sering kali berupa teks dengan opsi menu terbatas.
UEFI: UEFI menyediakan antarmuka pengguna yang lebih canggih, termasuk dukungan untuk grafis, mouse, dan perintah yang lebih maju. Ini membuatnya lebih mudah untuk mengonfigurasi sistem dan melihat informasi di layar BIOS.
Keamanan:

BIOS: BIOS memiliki fitur keamanan terbatas. Secara default, BIOS tidak memiliki mekanisme untuk memverifikasi integritas kode boot, yang dapat menyebabkan risiko keamanan.
UEFI: UEFI menyertakan fitur keamanan yang lebih baik, seperti Secure Boot, yang memverifikasi integritas kode boot dan perangkat lunak saat booting sistem. Ini membantu mencegah perangkat lunak berbahaya atau tidak sah dari dimuat selama proses boot.
Bootloader:

BIOS: BIOS menggunakan MBR (Master Boot Record) sebagai skema partisi dan memuat bootloader dari sektor awal hard disk.
UEFI: UEFI menggunakan partisi EFI (Extensible Firmware Interface) dan memuat bootloader dari sistem file yang terletak di partisi EFI.
Dukungan Perangkat Keras:

BIOS: BIOS memiliki dukungan terbatas untuk perangkat keras modern, terutama dalam hal kapasitas partisi dan driver.
UEFI: UEFI mendukung perangkat keras modern dengan lebih baik, termasuk kapasitas partisi yang lebih besar, driver yang lebih lengkap, dan kemampuan untuk boot dari perangkat penyimpanan GPT (GUID Partition Table).
