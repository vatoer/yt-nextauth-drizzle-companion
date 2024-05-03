Untuk mendaftarkan aplikasi OAuth di dasbor Google, ikuti langkah-langkah berikut:

1. **Login ke Console Pengembang Google**: Buka [Console Pengembang Google](https://console.developers.google.com/) dan login menggunakan akun Google Anda.
    
2. **Buat Proyek Baru (Opsional)**: Jika Anda belum memiliki proyek yang sesuai, Anda dapat membuat proyek baru dengan mengklik tombol "Buat Proyek" di bagian atas kanan dashboard.
    
3. **Pilih atau Buat Proyek**: Jika Anda memiliki beberapa proyek, pilih proyek yang ingin Anda gunakan dari menu dropdown di bagian atas kiri dashboard. Jika Anda membuat proyek baru, Anda akan dialihkan secara otomatis ke proyek tersebut.
    
4. **Buka Tab "Credentials"**: Di panel navigasi kiri, klik "Credentials" untuk membuka tab yang berisi semua kredensial untuk proyek Anda.
    
5. **Buat Kredensial Baru**: Klik tombol "Buat Kredensial" di bagian atas kanan halaman.
    
6. **Pilih Jenis Kredensial**: Dalam dropdown "Pilih jenis kredensial", pilih "ID klien OAuth".
    
7. **Konfigurasi ID Klien OAuth**: Isi informasi yang diminta, seperti nama aplikasi, deskripsi, dan URL situs web. Pastikan untuk memilih jenis aplikasi yang sesuai, misalnya "Aplikasi Web", "Aplikasi Android", atau "Aplikasi iOS".
    
8. **Tentukan URIs Otorisasi**: Di bagian "URI yang diperbolehkan untuk pengalihan", masukkan URI pengalihan yang akan digunakan oleh Google untuk mengirim kode otorisasi. Ini harus mencocokkan URI yang Anda tetapkan dalam konfigurasi NextAuth di aplikasi Anda.
    
9. **Simpan Kredensial**: Setelah mengisi semua informasi yang diperlukan, klik tombol "Buat" untuk membuat ID klien OAuth baru.
    
10. **Catat Kredensial**: Catat ID Klien dan Kunci Rahasia yang dihasilkan. Anda akan memerlukan informasi ini saat mengonfigurasi NextAuth di aplikasi Anda.
    

Setelah mendaftarkan aplikasi OAuth di dasbor Google, Anda dapat menggunakan ID klien dan kunci rahasia tersebut untuk mengonfigurasi NextAuth dalam aplikasi Next.js Anda untuk mengizinkan masuk dengan Google. Pastikan untuk mengikuti panduan Google tentang praktik terbaik keamanan dan privasi saat mengembangkan aplikasi yang menggunakan layanan OAuth mereka.