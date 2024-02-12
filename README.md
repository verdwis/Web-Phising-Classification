# Web-Phising-Classification

Web phishing adalah bentuk kejahatan dunia maya di mana penyerang menipu individu untuk memberikan informasi sensitif dengan menyamar sebagai entitas yang dapat dipercaya dalam komunikasi elektronik. Projek ini bertujuan untuk mengidentifikasi dan mengklasifikasikan situs web phishing menggunakan teknik Deep Learning, dengan menganalisis URL dan konten HTML untuk mendeteksi ciri-ciri phishing/penipuan seperti kesalahan pengejaan nama domain, subdomain yang mencurigakan, formulir yang meminta data sensitif, skrip mencurigakan, dan desain halaman, dikarenakan phishing detector tradisional hanya menggunakan URL saja.

Menurut laporan Indonesian Anti-Phishing Data Exchange (IDADX) untuk periode selama tahun 2023, **laporan url phishing tertinggi** terjadi pada **bulan Februari** sebanyak **15.050** dan terendah bulan **November sebanyak 1.729**. Menurut laporan terbaru dari **_Indonesian Anti-Phishing Data Exchange (IDADX)_** untuk periode **Oktober hingga Desember 2023, terdapat 8.161 laporan URL phishing**. Bulan Desember mencatat jumlah pelaporan phishing tertinggi dibandingkan bulan lainnya selama **Q4 2023**.

# Pengumpulan Dataset
Merupakan dataset yang terdiri dari 45,373 contoh, mewakili halaman web benign dan phishing secara merata. Setiap contoh mencakup berbagai elemen dokumen HTML seperti teks, hyperlink, gambar, tabel, daftar, dan berbagai komponen URL mulai dari subdomain hingga query. Terdapat dua file excel pada dataset ini, yakni URL.xlsx dan HTML.xlsx. Tiap file excel memiliki dua kolom, yakni ‘Category’ dan ‘Data’ Dataset ini terdiri dari data yang dikumpulkan dari Alexa.com untuk halaman web yang sah dan phishtank.com untuk halaman web phishing.

Link dataset: [Klik disini](https://drive.google.com/drive/folders/1RUUWq0dpp8orM0dhdYCsYCuPDG-5nvtU)



# EDA
Dataset terdiri dari :

Banyak baris dataset url 45373 dan kolom 2 
Banyak baris dataset html 45373 dan kolom 2

<img width="873" alt="image" src="https://github.com/verdwis/Web-Phising-Classification/assets/101826376/ea6e483d-9f9c-412a-8e49-d083ab2b65c3">

Dataset ini termasuk ke dalam data yang balance, karena ini terlihat dari perbedaan antara kategori phising (spam) dan kategori non-phishing (ham) hanya terdapat pada satu data saja

<img width="885" alt="image" src="https://github.com/verdwis/Web-Phising-Classification/assets/101826376/8abdfc13-c672-49df-b391-1827a8e328d5">

Berdasarkan pola yang diamati pada dataset, kategori phishing (spam) cenderung memiliki karakter yang panjang, sementara kategori non-phishing (ham) cenderung memiliki karakter yang pendek.

# Hasil dan Evaluasi

<img width="499" alt="image" src="https://github.com/verdwis/Web-Phising-Classification/assets/101826376/88ebc05b-393a-4d2e-9c18-fa5d8d61122a">

Dapat disimpulkan bahwa model ini memiliki performa yang sangat baik dalam klasifikasi. Hal ini terlihat dari nilai akurasi yang tinggi pada kedua set data pelatihan dan validasi, mencapai lebih dari 99%. Selain itu, nilai precision dan recall juga tinggi untuk kedua kategori, menunjukkan bahwa model memiliki kemampuan untuk mengidentifikasi dengan baik baik kelas positif (phishing) maupun kelas negatif (non-phishing). Secara umum, model ini telah berhasil dilatih dengan baik dan mampu memberikan prediksi yang andal untuk kasus klasifikasi phishing.

# Test Model

<img width="502" alt="image" src="https://github.com/verdwis/Web-Phising-Classification/assets/101826376/1a2a27ad-c9b0-4354-9b16-f7ae1737f052">



















