📦 CHECKPOINT #5 — TrackORA Web
Tanggal: 22 Juni 2026
Status Project: Frontend terintegrasi Google Sheets, progress bar dinamis 6 status, dashboard list, semua fitur berfungsi. Siap setup Power Automate.

🎯 Tujuan Project
Webapp TrackORA untuk melacak pengiriman unit mobil baru dari pusat distribusi → RVDC Ngoro → cabang. Data bersumber dari Google Sheets (via CSV publish), yang nantinya akan disinkronkan otomatis dari Excel via Power Automate.

🧰 Tools & URL
Tools	Fungsi
GitHub	Repository & version control
GitHub Pages	Hosting live & publik
Google Sheets	Database (CSV publish)
Power Automate	Sinkronisasi Excel → Sheets
Repo: https://github.com/maulinanda/trackora-web

Live: https://maulinanda.github.io/trackora-web/

Sheets CSV: https://docs.google.com/spreadsheets/d/e/2PACX-1vRKAaGXzzufPDknUNGa1u3sEEt_Py0lUS8PJKslvYt7b5Y5IgzklmLg10BkIz3uStTbR83hjinxZc7V/pub?gid=0&single=true&output=csv

📁 Struktur File
text
trackora-web/
├── README.md
└── index.html        ← HTML + CSS + JS (1 file)
🚗 6 Status Final
Angka	Status	Ikon	Progress Bar
0	Belum DR	⚪	Tidak muncul, banner "Belum DR"
1	DR Created	📝	Step 1 aktif
2	On Preparation	🔧	Step 2 aktif
3	Quality Reconditioning	✨	Step 3 (hanya jika QR terjadi)
4	In Transit	🚛	Step 4 aktif
5	Delivered	✅	Step 5 (disembunyikan sementara)
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
M	InTransit	Formula (nanti)
N	Delivered	Formula (nanti)
O	Status	Formula
📋 Semua Fitur
Fitur	Status
🔍 Lacak unit by No. Rangka	✅ Berfungsi
📋 Progress bar dinamis (QR opsional)	✅ Berfungsi
🚛 Info RVDC Ngoro di detail unit	✅ Berfungsi
📅 Estimasi tiba RVDC	✅ Berfungsi
🏢 Cabang Pemilik + Tujuan Kirim di detail	✅ Berfungsi
📊 Dashboard list + filter cabang	✅ Berfungsi
🔐 Login Admin PIN	✅ Berfungsi
💾 Sesi admin 30 menit (localStorage)	✅ Berfungsi
🛠️ Panel Admin (maju/reset/QR)	✅ Berfungsi
📱 Responsive mobile	✅ Berfungsi
🔗 Fetch data dari Google Sheets CSV	✅ Berfungsi
📅 Format tanggal fleksibel	✅ Berfungsi
⚡ Power Automate sinkronisasi	❌ Belum setup
🔜 Langkah Selanjutnya
Setup Power Automate — sinkronkan Excel (OneDrive) → Google Sheets

Test sinkronisasi — ubah data di Excel, lihat perubahan di webapp

Setup formula InTransit & Delivered di Google Sheets

Checkpoint #6 — dokumentasi setelah integrasi penuh

💡 Cara Melanjutkan di Chat Baru
Copy-paste checkpoint ini ke chat baru:

"Saya sedang membangun project TrackORA Web. Ini checkpoint #5. Semua fitur frontend berfungsi. Saya ingin lanjut setup Power Automate untuk sinkronisasi Excel ke Google Sheets."
