# HolyBytes AI Assistant

## Deskripsi

HolyBytes AI Assistant merupakan sebuah aplikasi web berbasis chat interaktif yang dirancang untuk memberikan pengalaman berkomunikasi dengan kecerdasan buatan secara alami dan bermanfaat. Aplikasi ini dikembangkan dengan penuh dedikasi oleh Ade Pratama dengan memanfaatkan teknologi mutakhir dari model Llama 3.3 70B Instruct melalui integrasi OpenRouter API.

## Fitur Utama

- **Antarmuka Percakapan yang Elegan**: Desain antarmuka yang intuitif dan responsif, memudahkan pengguna dalam berinteraksi dengan asisten AI
- **Manajemen Obrolan yang Fleksibel**: Kemampuan untuk membuat, menyunting judul, serta mengarsipkan percakapan sesuai kebutuhan
- **Panel Navigasi yang Praktis**: Akses mudah ke seluruh riwayat percakapan melalui panel samping yang dapat disesuaikan
- **Penyimpanan Data Lokal**: Seluruh percakapan disimpan secara aman di penyimpanan lokal peramban pengguna, menjamin privasi dan kenyamanan
- **Kecerdasan Buatan Berkualitas**: Didukung oleh model Llama 3 70B Instruct yang canggih melalui OpenRouter API untuk memberikan respons yang bernilai
- **Indikator Interaksi Real-time**: Visualisasi proses berpikir AI saat merespons permintaan pengguna
- **Pemformatan Pesan Lengkap**: Dukungan penyajian konten yang variatif termasuk kode program dan pemformatan teks
- **Desain Adaptif**: Tampilan yang optimal pada berbagai perangkat dan ukuran layar

## Teknologi yang Diterapkan

- **Frontend**: Dibangun dengan HTML, CSS, dan JavaScript murni
- **Desain Antarmuka**: Menggunakan framework Tailwind CSS
- **Ikon Visual**: Memanfaatkan koleksi Font Awesome
- **Penyimpanan Data**: Mengimplementasikan localStorage API
- **Kecerdasan Buatan**: Terintegrasi dengan OpenRouter API menggunakan model meta-llama/llama-3-70b-instruct

## Panduan Penggunaan

1. **Memulai Interaksi Baru**:
   - Tekan tombol "Percakapan Baru" pada panel samping
   - Aplikasi akan secara otomatis menyiapkan sesi baru saat pertama kali diakses

2. **Mengirimkan Pertanyaan**:
   - Masukkan pesan Anda pada kolom input di bagian bawah antarmuka
   - Kirim pertanyaan dengan menekan tombol kirim atau tombol Enter
   - Tunggu sejenak sambil asisten AI menyiapkan respons terbaik

3. **Mengelola Riwayat Percakapan**:
   - Akses panel navigasi melalui ikon menu di pojok kiri atas
   - Telusuri seluruh arsip percakapan yang tersimpan
   - Ketuk percakapan yang diinginkan untuk melanjutkan dialog
   - Gunakan opsi penyuntingan untuk mengubah judul percakapan
   - Fitur penghapusan tersedia untuk mengelola ruang penyimpanan

4. **Pemformatan Konten**:
   - Gunakan tanda `` untuk menyisipkan kode singkat
   - Manfaatkan ``` untuk menampilkan blok kode yang lebih kompleks

## Instalasi dan Konfigurasi

1. **Mengunduh Kode Aplikasi**:
   ```bash
   git clone https://github.com/HolyBytes/ai-assistant.git
   ```

2. **Menyiapkan Koneksi API**:
   - Buka berkas JavaScript utama
   - Temukan variabel `OPENROUTER_API_KEY`
   - Masukkan kredensial API OpenRouter Anda yang valid

3. **Menjalankan Aplikasi**:
   - Unggah seluruh berkas ke server web pilihan Anda
   - Untuk pengujian lokal, dapat menggunakan ekstensi Live Server pada VSCode

## Uji Coba Langsung

Anda dapat langsung mencoba HolyBytes AI Assistant melalui tautan berikut:  
🌐 [HolyBytes AI Assistant Demo](https://holybytes.github.io/HolyBytes-AI-Assistant/)

## Penyesuaian Aplikasi

### Pemilihan Model AI

Untuk menggunakan model AI alternatif, sesuaikan parameter berikut dalam fungsi `fetchAIResponse`:

```javascript
body: JSON.stringify({
    model: 'pilih-model-yang-diinginkan',
    messages: messages,
    temperature: 0.7,
    max_tokens: 2000
})
```

### Modifikasi Tampilan

Aplikasi mendukung penyesuaian antarmuka melalui Tailwind CSS dan CSS kustom. Anda dapat memodifikasi nilai dalam tag `<style>` sesuai preferensi desain.

## Aspek Keamanan dan Privasi

- Seluruh data percakapan disimpan secara eksklusif di perangkat pengguna
- Proses pengolahan pesan dilakukan melalui API OpenRouter yang terjamin
- Untuk implementasi produksi, disarankan menggunakan lapisan pengamanan tambahan untuk melindungi kredensial API

## Dukungan dan Kolaborasi

- Kunjungi repositori resmi kami: [HolyBytes GitHub](https://github.com/HolyBytes)
- Dukung pengembangan kami melalui: [Saweria HolyBytes](https://saweria.co/HolyBytes)

## Catatan Penting

- Aplikasi memerlukan koneksi internet dan API key OpenRouter yang aktif
- Penggunaan API mungkin memiliki ketentuan dan kebijakan tertentu dari penyedia
- Kapasitas penyimpanan lokal memiliki batasan teknis sesuai spesifikasi peramban

## Hak Cipta

© 2024 Ade Pratama. Seluruh hak cipta dilindungi undang-undang.

---

Terima kasih atas kepercayaan Anda menggunakan HolyBytes AI Assistant. Kami senantiasa berkomitmen untuk memberikan pengalaman berinteraksi dengan teknologi kecerdasan buatan yang bermanfaat dan menyenangkan. Untuk mencoba langsung, silakan kunjungi [halaman demo resmi kami](https://holybytes.github.io/HolyBytes-AI-Assistant/).
