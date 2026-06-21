📦 CHECKPOINT #7 — Branch fitur-multi-dan-admin
Tanggal: 22 Juni 2026
Status Project: Branch fitur-multi-dan-admin dengan fitur lengkap: multi input, navigasi detail↔daftar, admin mode dengan filter multi-select, tampilan rapi tanpa data sebelum aksi.

🎯 Tujuan Branch
Menggabungkan fitur multi No. Rangka dan daftar unit admin-only. Admin mode hanya untuk melihat daftar unit dengan filter per kolom. User biasa tetap bisa lacak 1 No. Rangka atau banyak unit.

🧰 Tools & URL
Tools	Fungsi
GitHub	Repository & version control
GitHub Pages	Hosting live (main branch)
HTML Preview	Testing branch lain
Google Sheets	Database (CSV publish)
Repo: https://github.com/maulinanda/trackora-web

Branch saat ini: fitur-multi-dan-admin

Live (main): https://maulinanda.github.io/trackora-web/

Preview branch: https://htmlpreview.github.io/?https://github.com/maulinanda/trackora-web/blob/fitur-multi-dan-admin/index.html

🚗 6 Status Final
Angka	Status	Ikon	Progress Bar
0	Belum DR	⚪	Tidak muncul, banner
1	DR Created	📝	Step 1
2	On Preparation	🔧	Step 2
3	Quality Reconditioning	✨	Step 3 (opsional)
4	In Transit	🚛	Step 4
5	Delivered	✅	Step 5 (sembunyi)
📊 Google Sheets — 15 Kolom
#	Header	Sumber
A	FrameNumber	Excel
B	BranchName	Excel
C	Model	Excel
D	Warna	Excel
E	AreaProcess	Excel
F	PermintaanSampaiCabang	Excel
G	TransactionDate	Excel
H	ETARVDC	Excel
I	ESTIMASI_SELESAI_REPAIR	Excel
J	TRUEDESTINATION	Excel
K	ESTIMASI_KIRIM_ADJUSTABLE	Excel
L	ETARVDC_Stat	Excel
M	InTransit	Formula
N	Delivered	Formula
O	Status	Formula
📋 Fitur di Branch fitur-multi-dan-admin
Fitur	Status
🔍 1 textarea untuk single/multi No. Rangka	✅
📋 Multi result tabel, klik → detail	✅
↩️ Navigasi detail ↔ daftar	✅
✕ Tombol Clear	✅
🔐 Admin Mode password Toyota2026	✅
📊 Daftar unit admin-only (min status 1)	✅
🔍 Filter No. Rangka (text)	✅
🏢 Filter Cabang Pemilik (text + datalist)	✅
🚗 Filter Model (multi-select dropdown)	✅
📝 Filter Status (multi-select dropdown)	✅
✕ Reset filter	✅
🙈 Data tersembunyi sebelum aksi	✅
🔒 Tab Lacak sembunyi saat Admin Mode	✅
📱 Responsive mobile	✅
🔜 Yang Belum
Item	Status
⚡ Power Automate (Excel → Sheets)	❌ Belum setup
📅 Formula InTransit & Delivered	❌ Menunggu data
🔀 Merge ke main	❌ Setelah evaluasi
💡 Cara Melanjutkan di Chat Baru
Copy-paste checkpoint ini:

"Saya sedang membangun project TrackORA Web. Ini checkpoint #7. Saya di branch fitur-multi-dan-admin. Semua fitur frontend berfungsi. Siap lanjut ke [Power Automate / merge / fitur lain]."
