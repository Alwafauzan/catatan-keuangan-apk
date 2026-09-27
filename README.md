# Catatan Keuangan

Aplikasi catatan keuangan pribadi untuk Android. Catat pemasukan, pengeluaran, dan
transfer antar akun - manual atau lewat AI (teks / suara).

> Repo ini khusus berisi **APK rilis**. Kode sumber aplikasi ada di repo terpisah
> dan di-build dari sana.

## Unduh

**[Download Catatan Keuangan v1.0.1](https://github.com/Alwafauzan/catatan-keuangan-apk/releases/download/v1.0.1/catatan-keuangan-1.0.1.apk)**

`catatan-keuangan-1.0.1.apk` - 48,7 MB

Halaman semua versi: <https://github.com/Alwafauzan/catatan-keuangan-apk/releases>

## Cara pasang

1. Unduh file `.apk` di atas.
2. Buka file-nya di HP (dari browser atau folder unduhan).
3. Android akan meminta izin **"pasang aplikasi tidak dikenal"** untuk aplikasi yang
   kamu pakai membuka file (Chrome / Files / Samsung Internet). Izinkan, lalu buka
   lagi file `.apk`-nya.
4. Di dalam app: **Daftar** pakai email kamu, lalu mulai catat transaksi.

Cara paling aman: buka link unduhan ini langsung di HP yang mau dipakai.

## Syarat minimum

- **Android 7.0 (Nougat)** atau lebih baru
- Koneksi internet - data disimpan di server, jadi app perlu online
- Akun yang dibuat lewat halaman Daftar di dalam app

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

## Data & privasi

- Setiap pengguna punya datanya sendiri; transaksi orang lain tidak bisa dilihat.
- Akun dibuat dengan email + kata sandi.
- Data disimpan di database PostgreSQL dengan akses dibatasi per pengguna.

## Update

Kalau ada versi baru, file `.apk` baru diunggah ke halaman
[Releases](https://github.com/Alwafauzan/catatan-keuangan-apk/releases) yang sama. Nama file dan
lokasinya tetap, jadi cukup cek halaman itu sesekali.

## Verifikasi file (SHA-256)

Untuk memastikan file yang kamu unduh asli dan tidak rusak / diubah di tengah jalan:

```
f367d8a67dfe3f7e42b5521046ddf5ba3fa3a1c5f9ce99821414699b650d3c15
```

Di HP, cek di Google Play dengan句 "APK & Bundle" > ikon tiga titik > "Tampilkan
checksum", lalu bandingkan dengan kode di atas.

## Lisensi

Proprietary. Repo ini hanya untuk distribusi binary; kode sumber tidak dipublikasikan.
