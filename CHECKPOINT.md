📦 CHECKPOINT #8 — Branch fitur-multi-dan-admin
Tanggal: 22 Juni 2026
Status Project: Branch fitur-multi-dan-admin dengan fitur lengkap: multi input, navigasi detail↔daftar, admin mode dengan filter per kolom + tombol clear individual, UI responsif (laptop horizontal wrap center, mobile label di atas field full width). Siap untuk evaluasi sebelum merge ke main.

🎯 Tujuan Branch
Menggabungkan multi No. Rangka dan daftar unit admin-only. Admin mode hanya untuk melihat daftar unit dengan filter yang bisa di-reset per field. User biasa tetap bisa lacak 1 atau banyak No. Rangka.

🧰 Tools & URL
Repo: https://github.com/maulinanda/trackora-web

Branch: fitur-multi-dan-admin

Live (main): https://maulinanda.github.io/trackora-web/

Preview branch: https://htmlpreview.github.io/?https://github.com/maulinanda/trackora-web/blob/fitur-multi-dan-admin/index.html

🚗 6 Status Final
Angka	Status	Ikon
0	Belum DR	⚪
1	DR Created	📝
2	On Preparation	🔧
3	Quality Reconditioning	✨
4	In Transit	🚛
5	Delivered	✅
📊 Google Sheets — 15 Kolom
A: FrameNumber, B: BranchName, C: Model, D: Warna, E: AreaProcess, F: PermintaanSampaiCabang, G: TransactionDate, H: ETARVDC, I: ESTIMASI_SELESAI_REPAIR, J: TRUEDESTINATION, K: ESTIMASI_KIRIM_ADJUSTABLE, L: ETARVDC_Stat, M: InTransit, N: Delivered, O: Status

📋 Fitur Branch fitur-multi-dan-admin
Fitur	Status
🔍 1 textarea untuk single/multi No. Rangka	✅
📋 Multi result tabel, klik → detail	✅
↩️ Navigasi detail ↔ daftar	✅
✕ Tombol Clear all	✅
🔐 Admin Mode password Toyota2026	✅
📊 Daftar unit admin-only (min status 1)	✅
🔍 Filter No. Rangka (text)	✅
🏢 Filter Cabang Pemilik (text + datalist)	✅
🚗 Filter Model (multi-select dropdown, sorted A-Z)	✅
📝 Filter Status (multi-select dropdown)	✅
✕ Reset semua filter	✅
🔘 Tombol clear individual di tiap field filter	✅
🙈 Data tersembunyi sebelum aksi	✅
🔒 Tab Lacak sembunyi saat Admin Mode	✅
📱 Responsive: laptop horizontal wrap center, mobile field full width	✅
🎨 Tampilan Filter
Laptop: label di atas field, field berukuran minimum 150px, wrap horizontal, align center, tombol reset di akhir baris.

Mobile: label di atas field, field full width, tombol reset rata kanan/stretch.

Setiap field input/select memiliki tombol ✕ kecil di samping kanan untuk clear isi field tersebut saja.

🔜 Rencana Selanjutnya
Power Automate — sinkronisasi Excel (OneDrive) → Google Sheets.

Formula InTransit & Delivered di Google Sheets.

Evaluasi — apakah fitur di branch ini layak digabung ke main.

Merge ke main — setelah puas dengan uji coba.
