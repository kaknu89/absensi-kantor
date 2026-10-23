# absensi-kantor

Halaman absensi untuk bot Telegram laporan kantor (Telegram Mini App).

Alur: tombol **🟢 Absen Masuk / 🔴 Absen Pulang** di bot → kamera depan terbuka otomatis →
hitung mundur 5 detik → foto diambil → lokasi diambil → dikirim ke server (Google Apps Script)
→ dikonfirmasi lewat Telegram (`sendData`) dari akun karyawan sendiri.

- Halaman ini **tidak menyimpan data** dan tidak berisi token/rahasia.
- Data absen hanya dikirim ke URL Web App Google Apps Script (`script.google.com/macros/s/.../exec`)
  yang tertera di link dari bot, dengan token bertanda tangan per karyawan.
- Foto & data absen tersimpan di Google Drive / Google Sheet perusahaan.
