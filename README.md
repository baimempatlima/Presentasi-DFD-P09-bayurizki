# Data Flow Diagram — Pertemuan 9

Presentasi web 51 slide untuk mata kuliah **Analisis dan Desain Sistem Informasi
Perpustakaan**, Jurusan Ilmu Perpustakaan, Fakultas Adab dan Humaniora,
UIN Alauddin Makassar.

Pengampu: Bayu Rizki, M.Kom · Bobot tugas 5 persen · CPMK-2, Sub-CPMK 4

## Menjalankan

Buka `index.html` di peramban. Tidak perlu pemasangan, tidak perlu internet —
fon sudah tertanam di dalam berkas, dan seluruh gambar ada di folder `img/`.

## Tombol

| Tombol | Fungsi |
|---|---|
| `→` `←` `Spasi` | Pindah slide |
| `Home` `End` | Ke slide pertama / terakhir |
| `O` | Ikhtisar 51 slide, klik untuk lompat |
| `F` | Layar penuh |
| Usap kiri/kanan | Pindah slide di ponsel atau tablet |

Tautan ke slide tertentu: tambahkan `#s34` di akhir alamat.

Kendali menghilang sendiri setelah 2,8 detik diam, jadi layar bersih saat mengajar.

## Menyalakan GitHub Pages

1. Tab **Settings** pada repositori ini
2. **Pages** di bilah kiri
3. **Source**: Deploy from a branch
4. Branch `main`, folder `/ (root)`, lalu **Save**

Tunggu build pertama selesai — lihat tab **Actions**, alur kerja
*pages build and deployment*. Saat centangnya hijau, situs hidup di
`https://<pengguna>.github.io/<nama-repo>/`

Kalau masih 404 sesudah hijau, muat ulang dengan `Ctrl+Shift+R` — 404 lama
tersimpan di cache peramban.

## Menyembunyikan slide

Setiap slide diberi komentar penanda di `index.html`, misalnya:

```html
<!-- ===== SLIDE 11 | Bagian F.3 · Dua Notasi DFD | Kotak atau bulat? ... ===== -->
<section class="slide">
```

Cari penandanya (Ctrl+F), lalu tambahkan kata `hide` pada kelasnya:

```html
<section class="slide hide">
```

Slide itu hilang dari presentasi, dari ikhtisar, dan dari hitungan. **Nomor
halaman ikut menyesuaikan sendiri** — tidak ada nomor yang lompat. Untuk
memunculkannya lagi, hapus kata `hide`.

Boleh juga dengan `data-hide`:

```html
<section class="slide" data-hide>
```

Cara ketiga: beri komentar pada seluruh blok slide, dari `<section ...>`
sampai `</section>` penutupnya. Hasilnya sama, hanya saja blok itu tidak
bisa dicari lagi dengan Ctrl+F sebagai slide.

Jangan mengubah angka pada komentar penanda — ia hanya petunjuk untuk mata
Anda, bukan dipakai program.

## Isi

| Berkas | Keterangan |
|---|---|
| `index.html` | Seluruh presentasi: 51 slide, gaya, fon tertanam, dan skrip navigasi |
| `img/` | 26 gambar DFD, dipakai apa adanya dari modul |
| `logo-uin.png` | Logo institusi |
| `.nojekyll` | Menyuruh GitHub Pages menyajikan berkas apa adanya |

## Catatan desain

Gaya *technical editorial / Swiss grid*: latar krem, rata kiri, garis rambut
sebagai pemisah, tanpa bayangan dan tanpa gradien.

- **Archivo 800** untuk judul, **Inter** untuk isi, **JetBrains Mono** untuk label
- Hijau `#248252` dan emas `#E1A835` diambil dari logo UIN Alauddin
- Rel di tepi kiri bukan hiasan: penanda emas bergeser turun mengikuti posisi
  slide, jadi terlihat sudah sampai mana dari 51
- Setiap gambar DFD duduk dalam bingkai putih bergaris tipis dengan label plat
  di sudutnya, seperti pelat gambar pada manual teknis

## Lisensi materi

Materi kuliah milik penulis. Gambar DFD dibuat untuk modul praktikum P09.
