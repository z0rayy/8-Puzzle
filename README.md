# 🧩 8‑Puzzle Solver (z0rayy)

Solusi untuk 8‑Puzzle problem (atau Sliding Tile Puzzle) dengan menggunakan algoritma A‑star (A*), termasuk deteksi papan unsolvable.

---

## 📘 Deskripsi

• Puzzle 3×3 berisi 8 ubin bernomor dan 1 kotak kosong.

• Tujuan: mencapai konfigurasi tujuan (1–8 berurutan dengan kosong di pojok kanan bawah) dari konfigurasi awal, menggunakan gerakan legal (atas, bawah, kiri, kanan).

• Solusi optimal dicapai via algoritma A*, meminimalkan jumlah gerakan.

---

## 🧠 Algoritma A*

1. Buat dua SearchNode untuk initial & twin.
2. Masukkan kedua ke priority queue berdasarkan moves + manhattan().
3. Loop:
   - Dequeue node berkost terendah.
   - Jika goal → solusi; hentikan.
   - Generate neighbors (exclude parent).
   - Masukkan neighbor baru ke queue.
4. Jika twin mencapai goal dulu → tidak solvable

---

## 🚀 Fitur

• Solusi Optimal dengan A*
Menemukan langkah minimal menggunakan algoritma A* dengan heuristik Hamming dan Manhattan.

• Cek Solvabilitas
Mendeteksi apakah puzzle bisa diselesaikan sebelum proses pencarian.

• Urutan Langkah Solusi
Menampilkan setiap langkah dari awal hingga kondisi akhir secara jelas.

• Deteksi Puzzle Tidak Terpecahkan
Memberi pesan Unsolvable puzzle jika puzzle tidak dapat diselesaikan.

• Struktur Kode Modular
Terpisah menjadi kelas Board dan Solver untuk kemudahan pengembangan.

---

## Kontribusi
Kontribusi sangat diterima! Jika Anda ingin menambah fitur atau memperbaiki bug, silakan buat pull request atau laporkan issue di repository ini.

