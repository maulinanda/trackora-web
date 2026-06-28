📦 CHECKPOINT #10 — TrackORA Web
Tanggal: 28 Juni 2026
Status Project: v4.0 — 7 status (termasuk Received), integrasi dengan sheet DELIVERY_LOG (check-in/check-out driver), progress bar 6 langkah, filter Status termasuk Received.

🎯 Tujuan Webapp
TrackORA Web — webapp untuk melacak status pengiriman unit mobil baru. Data diambil dari Google Sheets (db_Web), yang kini terhubung dengan sheet DELIVERY_LOG (data check-in/check-out driver via TrackORA Driver).

🧰 Tools & URL
Repo: https://github.com/maulinanda/trackora-web

Live: https://maulinanda.github.io/trackora-web/

Google Sheets CSV: https://docs.google.com/spreadsheets/d/e/2PACX-1vRKAaGXzzufPDknUNGa1u3sEEt_Py0lUS8PJKslvYt7b5Y5IgzklmLg10BkIz3uStTbR83hjinxZc7V/pub?gid=0&single=true&output=csv

🚗 7 Status Final
Angka	Status	Ikon	Badge
0	Belum DR	⚪	Abu-abu
1	DR Created	📝	Oranye
2	On Preparation	🔄	Biru
3	Prime Finishing	✨	Oranye dashed
4	In Transit	🚛	Hijau
5	Delivered	✅	Ungu
6	Received	🏁	Biru outline
📊 Google Sheets — db_Web (17 Kolom)
#	Kolom	Sumber
A	FrameNumber	Excel
B	BranchName	Excel
C	Model	Excel
D	Warna	Excel
E	AreaProcess	Excel
F	PermintaanSampaiCabang	Excel
G	TransactionDate	Excel
H	ETARVDC	Excel
I	ESTIMASI SELESAI REPAIR	Excel
J	TRUEDESTINATION	Excel
K	ESTIMASI KIRIM ADJUSTABLE	Excel
L	ETARVDC_Stat	Excel
M	InTransit	Array formula (XLOOKUP ke DELIVERY_LOG "Waktu Check In")
N	Delivered	Array formula (XLOOKUP ke DELIVERY_LOG "Waktu Check Out")
O	Received	Hard copy dari Excel
P	SJKB	Excel
Q	Status	Formula
📊 Google Sheets — DELIVERY_LOG (7 Kolom)
A	B	C	D	E	F	G
SJKB	Waktu Check In	GPS Check In	Waktu Check Out	GPS Check Out	Status Kirim	Timestamp Server
📋 Fitur TrackORA Web
Fitur	Status
🔍 Lacak unit (single & multi No. Rangka)	✅
📊 Daftar unit admin-only	✅
🔐 Admin Mode password Toyota2026	✅
🔍 Filter per kolom (No. Rangka, Cabang, Model, Status)	✅
🔘 Clear individual per field filter	✅
📝 Status: 0-6 (Belum DR s/d Received)	✅
📈 Progress bar 6 langkah	✅
🚛 Banner RVDC (oranye & biru)	✅
✨ Prime Finishing	✅
🏁 Received	✅
📱 Responsive mobile	✅
↩️ Navigasi detail ↔ daftar	✅
🔄 Data dari Google Sheets CSV	✅
🔜 Rencana Selanjutnya
Tracking real-time — auto-refresh data setiap beberapa menit

Notifikasi perubahan status — email/Telegram ke cabang

Dashboard statistik — jumlah unit per status

Login multi-user — admin cabang hanya lihat unitnya sendiri
