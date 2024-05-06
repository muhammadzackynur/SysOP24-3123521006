NAMA : MUHAMMAD ZACKY NUR SEPTIAN
NRP  : 3123521006

Perbedaan antara "swapping" dan "paging" terletak pada cara sistem operasi mengelola dan mentransfer data antara RAM dan media penyimpanan sekunder seperti hard disk atau SSD. Kedua teknik ini digunakan untuk mengelola memori virtual dalam sistem komputer.

Paging:

Paging adalah teknik manajemen memori di mana memori fisik dibagi menjadi blok-blok kecil yang disebut "halaman" (page) dengan ukuran tetap.
Memori virtual dari program atau proses juga dibagi menjadi unit-unit kecil yang disebut "frame" dengan ukuran yang sama dengan halaman fisik.
Sistem operasi menggunakan tabel pembagian memori (page table) untuk mencocokkan alamat virtual dengan alamat fisik, sehingga memungkinkan penggunaan memori virtual tanpa harus menyimpan seluruh proses dalam RAM sepanjang waktu.
Ketika program memerlukan akses ke data yang tidak ada di RAM, sistem operasi memuat halaman yang diperlukan dari media penyimpanan sekunder ke dalam RAM, dan sebaliknya.

Swapping:

Swapping adalah teknik manajemen memori di mana seluruh proses atau bagian dari proses dipindahkan secara keseluruhan dari RAM ke media penyimpanan sekunder dan sebaliknya.
Ini berarti seluruh ruang memori yang dialokasikan untuk proses tersebut dipindahkan, termasuk kode program, data, dan variabel.
Swapping biasanya digunakan ketika sistem operasi membutuhkan lebih banyak memori fisik daripada yang tersedia di RAM, sehingga beberapa proses harus disimpan di media penyimpanan sekunder untuk memberikan ruang bagi proses lainnya.
Proses swapping biasanya lebih lambat daripada paging karena melibatkan transfer besar dari data antara RAM dan media penyimpanan sekunder.

perbedaan utama antara paging dan swapping 

adalah pada tingkat detail bagaimana data dipindahkan antara RAM dan media penyimpanan sekunder. Paging fokus pada memindahkan unit kecil data (halaman) secara dinamis, sementara swapping melibatkan pemindahan seluruh proses antara RAM dan media penyimpanan sekunder
