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

- :contentReference[oaicite:8]{index=8}
- Fungsi hitung:
  - **dimension()**
  - **hamming()**
  - **manhattan()**
  - **isGoal()**
- Mendukung:
  - :contentReference[oaicite:9]{index=9}
  - :contentReference[oaicite:10]{index=10}
  - :contentReference[oaicite:11]{index=11}
- **Solver**:
  - :contentReference[oaicite:12]{index=12}
  - :contentReference[oaicite:13]{index=13}
  - :contentReference[oaicite:14]{index=14}

---

## ⚙️ Instalasi & Build

1. Clone repo:
   ```bash
   git clone https://github.com/z0rayy/8-Puzzle.git
   cd 8-Puzzle
