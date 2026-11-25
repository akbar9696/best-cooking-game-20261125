# Dossier — Dapur Kilat (best-cooking-game-20261125-0137)

## Ringkasan

**Dapur Kilat** adalah game masak orisinal yang berjalan di browser
desktop dari file statis, tanpa satu pun permintaan jaringan. Pemain
menjadi koki di sebuah dapur: pesanan muncul di papan, bahan diambil
dari meja, hidangan dirakit lapis demi lapis di atas piring, lalu
disajikan sebelum pelanggan kehabisan sabar.

## Yang terlihat di layar

- **Dapur**: dinding ubin dan meja kayu, suasana dapur yang hangat.
- **Papan Pesanan**: 3 tiket pesanan aktif, tiap tiket menunjukkan nama
  hidangan, harga, bahan yang dibutuhkan (dengan centang saat bahan
  sudah ada di piring), dan batang kesabaran pelanggan.
- **Meja Bahan**: 6 tempat bahan — Roti, Patty, Keju, Selada, Tomat,
  Saus — masing-masing digambar dengan CSS dan bisa diklik atau
  dipilih lewat keyboard (1–6).
- **Piring Racikan**: tumpukan hidangan yang sedang dirakit
  (mid-assembly), dengan tombol SAJIKAN (menyala saat piring cocok
  dengan pesanan) dan BUANG.
- **Timer**: batang waktu 120 detik per ronde + hitung mundur tiap
  pesanan.
- **Piring siap disajikan**: saat susunan piring sama persis dengan
  pesanan, tombol SAJIKAN menyala kuning dan pesan "Siap!" muncul.

## Cara main

1. Baca pesanan di Papan Pesanan.
2. Klik bahan di meja (atau tekan 1–6) untuk menumpuknya di piring.
   Klik lapisan di piring untuk melepas bahan itu.
3. Tekan SAJIKAN (atau Enter) saat piring cocok persis dengan salah
   satu pesanan.
4. Sajikan sebelum kesabaran pesanan habis. Bonus kecepatan sampai
   +$50. Sajikan beruntun tanpa kesalahan untuk pengali kombo (x2,
   x3, ...).
5. Pesanan yang kedaluwarsa akan kabur dan kombo kembali ke x1.
   Tombol BUANG / Backspace mengosongkan piring.

## Hidangan & harga

| Hidangan | Bahan | Harga |
|---|---|---|
| Burger Klasik | Roti, Patty, Keju, Selada, Tomat | $120 |
| Cheeseburger | Roti, Patty, Keju ×2 | $100 |
| Salad Segar | Selada, Tomat, Keju, Saus | $90 |
| Sandwich Kilat | Roti, Selada, Tomat, Keju, Saus | $110 |
| Double Patty | Roti, Patty ×2, Keju, Selada | $150 |

Skor = harga hidangan + bonus kecepatan, dikali kombo aktif.

## Teknologi

- Satu file `index.html` (HTML + CSS + JavaScript sebaris, ~26 KB).
- Nol permintaan jaringan: tanpa CDN, font eksternal, gambar
  eksternal, atau API. Semua visual digambar dengan CSS.
- Efek suara memakai WebAudio (nada pendek hasil sintesis, tanpa
  file audio). Tanpa suara pun game tetap lengkap.
- Dimainkan dengan keyboard dan mouse; layout tetap 1280×800.
- Parameter `?shot=start|play|serve|done` menampilkan keadaan
  panggung yang sama dengan gameplay nyata, dipakai untuk mengambil
  screenshot dossier ini (bukan jalur permainan terpisah).

## Screenshot

| File | Isi |
|---|---|
| `screenshots/3-start.png` | Layar judul "DAPUR KILAT" di atas dapur |
| `screenshots/2-play.png` | Burger Klasik di tengah perakitan (Roti + Patty + Keju di piring), 3 pesanan aktif, timer 87 dtk |
| `screenshots/1-serve.png` | Piring lengkap cocok dengan Burger Klasik, tombol SAJIKAN menyala "Siap disajikan!" |
| `screenshots/4-done.png` | Layar akhir ronde: skor $1250, 9 hidangan, kombo terbaik x4 |

## Orisinalitas

Seluruh kode, nama hidangan, dan desain visual dibuat baru untuk
bounty ini. Tidak memakai aset, template, atau kode pihak ketiga.
