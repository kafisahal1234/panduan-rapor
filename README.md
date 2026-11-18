# Panduan Rapor Santri — Kampung Qur'an Al Muawanah

Website panduan pembuatan **10 slide Rapor Santri** untuk santri kelas 7–9.
Pembimbing: Ustadz M. Kafi Sahal Muhtar.

## Cara menghidupkan website ini (GitHub Pages)

1. Buat repository baru di GitHub, nama bebas, misalnya `panduan-rapor`.
   **Pilih Public** — kalau Private, GitHub Pages tidak jalan di akun gratis.
2. Di halaman repository, klik **Add file → Upload files**.
3. Tarik berkas `index.html` dan `.nojekyll` ke kotak upload, lalu **Commit changes**.
4. Masuk **Settings → Pages**.
5. Bagian *Source* pilih **Deploy from a branch**, *Branch* pilih **main**, folder **/ (root)**, klik **Save**.
6. Tunggu 1–2 menit, refresh halaman itu. Alamat website muncul di atas:
   `https://NAMA-AKUN.github.io/panduan-rapor/`

Alamat itu yang dibagikan ke santri. Gratis, tanpa login, bisa dibuka
berapa orang pun sekaligus.

## Cara memperbarui isinya

Buka `index.html` di GitHub → ikon pensil → ubah → **Commit changes**.
Perubahan muncul di website sekitar satu menit kemudian.

Untuk perubahan besar, gunakan paket Claude Code
(`panduan-rapor-untuk-claude-code.zip`) di komputer, lalu timpa `index.html`
di sini dengan hasil `dist/index.html`.

## Isi berkas

| Berkas | Keterangan |
|---|---|
| `index.html` | Seluruh website dalam satu berkas — HTML, CSS, JS, dan foto pembimbing sudah tertanam di dalamnya |
| `.nojekyll` | Memberi tahu GitHub Pages agar tidak memproses berkas, cukup sajikan apa adanya |

Satu-satunya berkas dari luar yang dimuat adalah pustaka jsPDF dari
cdnjs.cloudflare.com, dipakai saat santri mengunduh prompt menjadi PDF.

## Catatan

- Website ini **hanya membuat prompt**. Pembuatan file PPT dilakukan di AI
  eksternal (Gemini, ChatGPT, atau Claude) dengan menempelkan prompt tersebut.
- Jawaban santri tersimpan di peramban masing-masing (localStorage), jadi
  tidak hilang kalau halaman tertutup. Tidak ada data yang dikirim ke server.
- Rubrik penilaian tidak disertakan — itu wewenang guru.
