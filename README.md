# Jawaban-quis-1-Struktur-Data-Array-dan-Linked-List
1. Karakteristik Memori dan Akses Data
Array memiliki akses data dengan kompleksitas waktu O(1) karena data disimpan secara berurutan (kontinu) di memori. Setiap elemen memiliki indeks sehingga alamat memori dapat dihitung langsung. Oleh karena itu, elemen dapat diakses tanpa menelusuri data lain.

Sedangkan pada Single Linked List, data disimpan secara tidak berurutan (non-kontinu). Setiap node hanya memiliki data dan pointer ke node berikutnya. Untuk mencari elemen tertentu harus menelusuri node satu per satu dari awal sehingga kompleksitas ketersediaan O(n).

2. Analisis Efisiensi Operasi Manipulasi
Linked List lebih unggul dibandingkan Array pada operasi penyisipan dan penghapusan ketika data sering berubah atau penyisipan dilakukan di tengah data.

Pada Array, penyisipan dan penghapusan memerlukan pergeseran elemen sehingga membutuhkan waktu O(n). Sedangkan pada Linked List cukup mengubah pointer antar node tanpa memindahkan data lain. Jika posisi node sudah diketahui maka operasi dapat dilakukan dalam O(1).

3. Konsep Daftar Berantai Ganda
Node pada Double Linked List terdiri dari:

Data
Penunjuk selanjutnya
Penunjuk sebelumnya
Pointer tambahan membuat penggunaan memori lebih besar dibandingkan Single Linked List. Namun, penelusuran dapat dilakukan dua arah, maju dan mundur, sehingga lebih fleksibel dan mempermudah operasi penghapusan.

4. Mekanisme Linked List Melingkar
Circular Linked List memiliki node terakhir yang menunjuk kembali ke node pertama sehingga membentuk lingkaran. Berbeda dengan Linked List biasa yang node terakhirnya bernilai NULL.

Contoh penggunaan Circular Linked List adalah sistem Round Robin Scheduling karena proses dapat berjalan terus menerus secara bergiliran.

5. Array Dinamis di Python
Daftar Python menggunakan Dynamic Array. Ketika kapasitas penuh saat append dilakukan, Python akan membuat array baru dengan ukuran lebih besar lalu menyalin seluruh data dari array lama ke array baru.

Proses ini memerlukan waktu O(n) karena data harus dikontrol ulang, tetapi penambahan tetap dianggap O(1) secara rata-rata (diamortisasi).
