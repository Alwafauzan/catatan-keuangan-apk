# Catatan Keuangan

Aplikasi catatan keuangan pribadi untuk Android. Catat pemasukan, pengeluaran, dan
transfer antar akun - manual atau lewat AI (teks / suara).

> Repo ini khusus berisi **APK rilis**. Kode sumber aplikasi ada di repo terpisah
> dan di-build dari sana.

## Unduh

Pilih satu sesuai HP kamu. Hampir semua HP sekarang pakai **arm64**.

| Pilihan | Ukuran | Untuk siapa |
| --- | --- | --- |
| **[arm64 - 17,6 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan-arm64-v8a.apk)** | 18.447.324 byte | Xiaomi, Samsung, OPPO, Realme, vivo, Honor, dan sejenisnya. **Paling disarankan.** |
| **[armv7 - 14,9 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan-armeabi-v7a.apk)** | 15.675.816 byte | HP lama berprosessor 32-bit |
| **[Semua HP - 49,8 MB](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/latest/download/catatan-keuangan.apk)** | 52.175.426 byte | Kalau tidak yakin HP kamu yang mana |

Ketiganya sudah **versi 1.0.2**.

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

Menu **Input Manual**, **Input AI**, dan **Master Data** tersedia lewat tombol `+`
di layar utama.

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
Cocokkan dengan nilai di Google Play:

```
arm64      4b1ce5aef10ca251cae0831f13b20cb0ffd84e129cfacd7449f35ee036d59063
armv7      29363365e07ca1265d0d6cf5b6ebb3b7e04e4607b0154e03912136be3ef4c1b3
universal  ff40d298aa55da1ca0648aa44b9ca53bd4b7c0d2d8ca4109e6955ecf13987890
```

Di HP, cek di Google Play dengan "APK & Bundle" > ikon tiga titik > "Tampilkan
checksum", lalu bandingkan dengan kode di atas.

## Data & privasi

- Setiap pengguna punya datanya sendiri; transaksi orang lain tidak bisa dilihat.
- Akun dibuat dengan email + kata sandi.
- Data disimpan di database PostgreSQL dengan akses dibatasi per pengguna.

## Lisensi

Proprietary. Repo ini hanya untuk distribusi binary; kode sumber tidak dipublikasikan.
