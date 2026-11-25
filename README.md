# Dapur Kilat — Cooking Game

Game masak orisinal buat bounty make.fun **"Make the best cooking game"**
(`best-cooking-game-20261125-0137`).

## Main

Buka `index.html` di browser desktop — satu file statis, **tanpa
permintaan jaringan sama sekali**. Bisa juga disajikan lewat server
statis apa pun (`python3 -m http.server`, `npx serve`, dsb).

## Cara main

1. Baca pesanan di **Papan Pesanan** — tiap hidangan butuh bahan tertentu.
2. Klik bahan di **Meja Bahan** (atau tekan **1–6**) untuk menumpuknya
   di piring. Klik lapisan di piring untuk melepasnya.
3. Kalau piring sudah sama persis dengan salah satu pesanan, tekan
   **SAJIKAN** (atau **Enter**).
4. Sajikan sebelum kesabaran pelanggan habis — makin cepat, makin
   besar bonus. Sajikan beruntun tanpa salah untuk kombo berlipat.

Kontrol: **1–6** pilih bahan · **Enter** sajikan · **Backspace** buang
isi piring · **R** mulai ulang.

## Hidangan

| Hidangan | Bahan | Harga |
|---|---|---|
| Burger Klasik | Roti, Patty, Keju, Selada, Tomat | $120 |
| Cheeseburger | Roti, Patty, Keju ×2 | $100 |
| Salad Segar | Selada, Tomat, Keju, Saus | $90 |
| Sandwich Kilat | Roti, Selada, Tomat, Keju, Saus | $110 |
| Double Patty | Roti, Patty ×2, Keju, Selada | $150 |

Satu ronde: 120 detik, maksimal 3 pesanan aktif. Pesanan yang
kesabarannya habis akan kabur dan kombo reset.

## Screenshot

`screenshots/` berisi 4 tangkapan gameplay (1280×800):

- `3-start.png` — layar judul di atas dapur
- `2-play.png` — hidangan di tengah perakitan
- `1-serve.png` — piring lengkap, siap disajikan
- `4-done.png` — layar akhir ronde

Detail lengkap ada di `DOSSIER.md`.

## Lisensi

MIT — lihat `LICENSE`.
