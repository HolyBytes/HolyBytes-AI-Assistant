# HolyBytes AI Assistant

## Deskripsi

HolyBytes AI Assistant adalah aplikasi web interaktif yang menyediakan asisten AI berbasis chat. Aplikasi ini dikembangkan oleh ADE PRATAMA dan memanfaatkan teknologi AI dari Llama 3.3 70B Instruct melalui OpenRouter API untuk memberikan respons yang cerdas dan natural terhadap pertanyaan pengguna.

## Fitur Utama

- **Antarmuka Chat yang Interaktif**: Desain antarmuka yang bersih dan responsif, memungkinkan pengguna untuk berkomunikasi dengan mudah dengan asisten AI.
- **Manajemen Percakapan**: Kemampuan untuk membuat, mengganti nama, dan menghapus percakapan.
- **Sidebar Navigasi**: Navigasi mudah antara percakapan yang berbeda melalui sidebar yang dapat dibuka dan ditutup.
- **Penyimpanan Lokal**: Semua percakapan disimpan di localStorage browser pengguna, memastikan privasi dan akses cepat ke percakapan sebelumnya.
- **Respons AI Berkualitas Tinggi**: Memanfaatkan model Llama 3 70B Instruct yang canggih melalui API OpenRouter untuk memberikan respons yang informatif dan natural.
- **Indikator Mengetik**: Animasi saat AI sedang memproses permintaan pengguna.
- **Formatting Pesan**: Dukungan untuk kode dan pemformatan teks dasar dalam pesan.
- **Desain Responsif**: Tampilan yang optimal di berbagai perangkat, baik desktop maupun mobile.

## Teknologi yang Digunakan

- **Frontend**: HTML, CSS, JavaScript (Vanilla JS)
- **Styling**: Tailwind CSS
- **Icons**: Font Awesome
- **Storage**: Browser localStorage API
- **AI Backend**: OpenRouter API dengan model meta-llama/llama-3-70b-instruct

## Cara Penggunaan

1. **Memulai Percakapan Baru**:
   - Klik tombol "Chat Baru" di sidebar atau
   - Aplikasi secara otomatis membuat percakapan baru saat pertama kali dijalankan

2. **Mengirim Pesan**:
   - Ketik pesan di area input di bagian bawah layar
   - Tekan Enter atau klik ikon kirim untuk mengirim pesan
   - Tunggu respons dari asisten AI

3. **Mengelola Percakapan**:
   - Buka sidebar dengan mengklik ikon menu di kiri atas
   - Lihat semua percakapan tersimpan
   - Klik pada percakapan untuk beralih ke percakapan tersebut
   - Gunakan tombol edit untuk mengganti nama percakapan
   - Gunakan tombol hapus untuk menghapus percakapan

4. **Format Pesan**:
   - Gunakan `` untuk kode inline
   - Gunakan ``` untuk blok kode multi-baris

## Instalasi dan Pengaturan

1. **Clone atau download repository**:
   ```
   git clone https://github.com/HolyBytes/ai-assistant.git
   ```

2. **Konfigurasi API Key**:
   - Buka file JavaScript dan temukan variabel `OPENROUTER_API_KEY`
   - Ganti dengan API key OpenRouter Anda sendiri

3. **Deploy**:
   - Upload file ke server web atau
   - Jalankan di localhost dengan server web sederhana seperti Live Server di VSCode

## Kustomisasi

### Mengubah Model AI

Untuk menggunakan model AI yang berbeda, ubah parameter `model` dalam fungsi `fetchAIResponse`:

```javascript
body: JSON.stringify({
    model: 'nama-model-yang-diinginkan',
    messages: messages,
    temperature: 0.7,
    max_tokens: 2000
})
```

### Mengubah Tampilan

Aplikasi menggunakan Tailwind CSS dan custom CSS. Anda dapat mengubah nilai dalam tag `<style>` untuk menyesuaikan tampilan sesuai kebutuhan Anda.

## Pertimbangan Privasi dan Keamanan

- Semua data percakapan disimpan secara lokal di browser pengguna menggunakan localStorage
- Pesan dikirim ke API OpenRouter untuk diproses
- API key disimpan di sisi klien; untuk penggunaan produksi, sebaiknya gunakan proxy server untuk melindungi API key

## Dukungan dan Kontribusi

- Kunjungi repositori GitHub: [https://github.com/HolyBytes](https://github.com/HolyBytes)
- Dukung pengembang melalui: [https://saweria.co/HolyBytes](https://saweria.co/HolyBytes)

## Keterbatasan

- Aplikasi membutuhkan API key OpenRouter yang valid
- Penggunaan API mungkin tunduk pada batasan dan biaya sesuai kebijakan penyedia
- Penyimpanan lokal memiliki batasan ukuran; percakapan yang sangat panjang dapat melebihi batas localStorage browser

## Lisensi

© 2024 ADE PRATAMA

---

Terima kasih telah menggunakan HolyBytes AI Assistant! Kami berharap aplikasi ini membantu meningkatkan produktivitas dan memberikan pengalaman interaksi dengan AI yang menyenangkan.
