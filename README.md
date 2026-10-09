# SoundRip

SoundRip adalah aplikasi web statis untuk mengonversi audio dari file video atau audio ke format MP3. Seluruh proses berlangsung secara lokal di browser: file tidak diunggah ke server, tidak memerlukan akun, dan dapat dibuka tanpa koneksi internet setelah halaman dimuat.

## Fitur

- Konversi lokal ke MP3 dengan pilihan bitrate 96–320 kbps.
- Pilihan keluaran stereo atau mono.
- Drag-and-drop, indikator kemajuan, dan waveform audio.
- Tanpa backend, database, analitik, atau API key.
- Siap dihosting di GitHub Pages karena proyek hanya memakai HTML, CSS, dan JavaScript.

## Cara menggunakan

1. Buka `index.html` di browser modern, atau kunjungi halaman GitHub Pages setelah dipublikasikan.
2. Pilih atau seret satu file video/audio.
3. Tentukan bitrate dan channel.
4. Klik **KONVERSI KE MP3**, lalu unduh hasilnya.

## Menjalankan secara lokal

Tidak ada proses instalasi atau dependensi.

```text
[Klik untuk Membuka](https://andros38.github.io/SoundRIP/)
atau bisa copy link dibawah ini :
https://andros38.github.io/SoundRIP/
```

Untuk pengembangan, proyek ini juga dapat dilayani oleh static server apa pun. Namun, server tidak diperlukan untuk penggunaan normal.

## Publikasi di GitHub Pages

1. Buat repositori GitHub baru, misalnya `soundrip`.
2. Unggah seluruh isi folder ini ke cabang `main`. Pastikan `index.html` berada di direktori utama repositori.
3. Buka **Settings → Pages** pada repositori.
4. Pada **Build and deployment**, pilih **Deploy from a branch**, lalu pilih `main` dan folder `/(root)`.
5. Simpan. GitHub akan menampilkan alamat publiknya setelah proses deploy selesai.

## Batasan teknis

- Dukungan file input ditentukan oleh codec yang tersedia pada browser dan sistem operasi, bukan hanya ekstensi file. MP4, WebM, MP3, dan WAV umumnya paling aman, tetapi hasil dapat berbeda antarperangkat.
- File besar memerlukan RAM karena proses decoding dan encoding dilakukan di perangkat pengguna. Gunakan browser terbaru dan tutup tab lain bila konversi terasa berat.
- Aplikasi ini membuat MP3 dari media lokal; gunakan hanya untuk file yang Anda miliki atau berhak Anda olah.

## Struktur proyek

```text
.
├── index.html                 # Aplikasi lengkap, termasuk encoder lokal
├── README.md                  # Dokumentasi penggunaan dan GitHub Pages
├── LICENSE                     # Lisensi kode asli SoundRip (MIT)
├── THIRD_PARTY_NOTICES.md      # Atribusi encoder pihak ketiga
├── SECURITY.md                 # Cara melaporkan masalah keamanan
├── .gitignore
└── .gitattributes
```

## Lisensi

Kode asli SoundRip dilisensikan di bawah [MIT License](LICENSE). Proyek juga memuat encoder pihak ketiga; ketentuan dan atribusinya tersedia di [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

