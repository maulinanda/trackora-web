📦 CHECKPOINT #9 — TrackORA Web
Tanggal: 23 Juni 2026
Status Project: Branch main stabil dengan fitur lengkap. Branch ui-ux-iteration dengan tampilan corporate modern. Branch fitur-login siap dibuat.

🎯 Tujuan Project
Webapp TrackORA untuk melacak pengiriman unit mobil baru dari pusat distribusi → RVDC Ngoro → cabang. Digunakan oleh orang cabang (lacak unit) dan admin cabang (login + daftar unit + filter).

🌿 Branch Saat Ini
Branch	Status	Deskripsi
main	✅ Production	Fitur lengkap: multi No. Rangka, daftar unit, filter, banner RVDC, Prime Finishing
ui-ux-iteration	🎨 Aktif	Tampilan corporate modern (navbar, font Inter, palet monokromatik, stepper minimalis)
fitur-login	🔜 Segera dibuat	Login admin cabang (email + password), akses terbatas per cabang
🧰 Tools & URL
Repo: https://github.com/maulinanda/trackora-web

Live (main): https://maulinanda.github.io/trackora-web/

Google Sheets CSV: https://docs.google.com/spreadsheets/d/e/2PACX-1vRKAaGXzzufPDknUNGa1u3sEEt_Py0lUS8PJKslvYt7b5Y5IgzklmLg10BkIz3uStTbR83hjinxZc7V/pub?gid=0&single=true&output=csv

🚗 6 Status Final
Angka	Status	Ikon
0	Belum DR	⚪
1	DR Created	📝
2	On Preparation	🔄
3	Prime Finishing	✨
4	In Transit	🚛
5	Delivered	✅
📋 Fitur di Branch main
Fitur	Status
🔍 Lacak unit (single & multi No. Rangka)	✅
📊 Daftar unit admin-only	✅
🔐 Admin Mode password Toyota2026	✅
🔍 Filter per kolom (No. Rangka, Cabang, Model, Status)	✅
🔘 Clear individual per field filter	✅
🚛 Banner RVDC (oranye & biru)	✅
✨ Prime Finishing (sebelumnya Quality Reconditioning)	✅
📱 Responsive mobile	✅
↩️ Navigasi detail ↔ daftar	✅
🔄 Sinkronisasi via Google Sheets CSV	✅
🎨 Tampilan di Branch ui-ux-iteration
Komponen	Perubahan
Warna	Monokromatik: navy #0F172A, abu #F1F5F9, biru #2563EB
Font	Inter / system-ui
Kartu	Border tipis, shadow minimal
Progress bar	Stepper 28px, animasi pulse-ring
Badge status	Outline style, lebih subtle
Tabel	Garis tipis, hover halus
Filter	Border 1px, focus ring
Popup login	Shadow dalam, backdrop blur
Banner	Background solid, tanpa border kiri tebal
🔜 Rencana Branch fitur-login
Fitur	Detail
Login	Email + password unik per admin cabang
Database user	Hardcode di JavaScript (sederhana)
Akses	Admin hanya lihat unit di cabangnya sendiri
User biasa	Tetap bisa lacak unit tanpa login
Sesi	localStorage 30 menit
💡 Cara Melanjutkan
Buat branch fitur-login dari ui-ux-iteration

Kirimkan database email & password admin

Mulai coding fitur login
