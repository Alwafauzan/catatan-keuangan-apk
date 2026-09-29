# Catatan Keuangan

Aplikasi catatan keuangan pribadi untuk Android. Catat pemasukan, pengeluaran, dan
transfer antar akun - manual atau lewat AI (teks / suara).

> Repo ini khusus berisi **APK rilis**. Kode sumber aplikasi ada di repo terpisah
> dan di-build dari sana.

## Unduh

Pilih satu sesuai HP kamu. Hampir semua HP sekarang pakai **arm64**.

| Pilihan | Ukuran | Untuk siapa |
| --- | --- | --- |
| **[arm64 - 17,7 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan-arm64-v8a.apk)** | 18.580.020 byte | Xiaomi, Samsung, OPPO, Realme, vivo, Honor, dan sejenisnya. **Paling disarankan.** |
| **[armv7 - 15,2 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan-armeabi-v7a.apk)** | 15.923.200 byte | HP lama berprosessor 32-bit |
| **[Semua HP - 50,3 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan.apk)** | 52.750.490 byte | Kalau tidak yakin HP kamu yang mana |

Ketiganya sudah **versi 1.0.4**.

Ada juga `catatan-keuangan-x86_64.apk` (20.129.332 byte) untuk emulator atau
HP yang benar-benar 32-bit. Jarang perlu — hampir semua HP sekarang sudah arm64.

Halaman semua versi: <https://github.com/Alwafauzan/catatan-keuangan-apk/releases>

## Cara pasang

1. Unduh file `.apk` dari salah satu tombol di atas.
2. Buka file-nya di HP (dari browser atau folder unduhan).
3. Android akan meminta izin **"pasang aplikasi tidak dikenal"** untuk aplikasi yang
   kamu pakai membuka file (Chrome / Files / Samsung Internet). Izinkan sekali saja,
   lalu buka lagi file `.apk`-nya.
4. Di dalam app: **Daftar** pakai email kamu, lalu mulai catat transaksi.

Cara paling aman: buka halaman ini langsung di HP yang mau dipakai, lalu ketuk tombol unduh.

## Syarat minimum

- **Android 7.0 (Nougat)** atau lebih baru
- Koneksi internet - data disimpan di server, jadi app perlu online
- Akun yang dibuat lewat halaman Daftar di dalam app
- Sekitar 100 MB ruang kosong

## Fitur

- **Dashboard** - total saldo, saldo per akun, pemasukan & pengeluaran bulan ini
- **Input manual** - form lengkap dengan validasi, plus peringatan kalau saldo kurang
- **Transfer antar akun** - termasuk biaya admin (dibayar pengirim / dipotong penerima)
- **Filter transaksi** - berdasarkan rentang tanggal, tipe, dan kategori
- **Master data** - tambah / edit / hapus akun (bank, e-wallet, tunai) dan kategori
- **Input AI** - tulis kalimat biasa ("beli cilok 5rb pakai BCA") atau rekam suara,
  lalu form terisi otomatis; tetap bisa kamu cek & ubah sebelum disimpan
- **Ubah kata sandi** - ganti kata sandi langsung dari dalam aplikasi (versi 1.0.3)
- **Premium QRIS** - langganan dengan kuota AI tanpa batas, dibayar lewat QRIS yang
  nominalnya sudah menempel di dalam QR jadi tidak ada salah nominal (versi 1.0.4)

Menu **Input Manual**, **Input AI**, dan **Master Data** tersedia lewat tombol `+`
di layar utama. Tombol **Premium** ada di kanan atas.

## Update

Sejak versi 1.0.2, aplikasi **mengecek update sendiri**. Begitu ada versi baru,
muncul notifikasi di dalam app: unduh, periksa checksum, lalu buka installer.

- Tombol **"Cek Update"** ada di layar utama kalau mau memeriksa manual.
- Update biasa bisa ditutup. Update yang *wajib* (versi lama sudah rusak) tidak bisa
  ditutup sampai selesai. Keduanya tetap butuh persetujuan "Install" dari sistem Android.
- Rilisan 1.0.1 ke bawah belum punya mekanisme ini, jadi harus unduh manual
  sekali ke 1.0.2. Setelah itu, update berikutnya otomatis.

Semua tautan unduh di README dan di
[halaman download](https://alwafauzan.github.io/catatan-keuangan/) memakai
`releases/latest/download/`, jadi **tidak perlu diubah setiap rilis baru** - GitHub
otomatis mengarahkan ke berkas terbaru.

## Verifikasi file (SHA-256)

Untuk memastikan file yang kamu unduh asli dan tidak rusak / diubah di tengah jalan.
Buka halaman [rilis terbaru](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest),
scroll ke bagian `Assets`, lalu cocokkan ukuran file dengan tabel di atas.

Hash versi **1.0.4** (yang sedang diunduh lewat `latest/download`):

```
arm64      45837fa67e7d7ea89433c1f4af790cb53fd0ef7f31d0c5bb82893f1a075c58ef
armv7      366b32c66835bc600726fa0a3b7b888169a90bb53a3318c93fbcfa357da1541f
x86_64     d9e6525d55b57ded3980de10c3a9c966b0dcec33041442f8f453082c7dd07d76
universal  4cde42240900df545df58d2d80807be8ca8cf2d3a498a9bfc9d00c9dd6acd6de
```

Aplikasi juga memeriksa hash-nya sendiri sebelum membuka installer, jadi file yang
salah atau terpotong akan ditolak dengan pesan jelas, bukan dipasang diam-diam.

## Data & privasi

- Setiap pengguna punya datanya sendiri; transaksi orang lain tidak bisa dilihat.
- Akun dibuat dengan email + kata sandi.
- Data disimpan di database PostgreSQL dengan akses dibatasi per pengguna.

## Lisensi

Proprietary. Repo ini hanya untuk distribusi binary; kode sumber tidak dipublikasikan.
