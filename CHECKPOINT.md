📦 CHECKPOINT #3 — TrackORA Web
Tanggal: 20 Juni 2026
Status Project: Frontend lengkap dengan Dashboard, Search, Filter, Stats, Admin Mode, dan Quality Reconditioning dinamis. Siap masuk fase backend.

🎯 Tujuan Project
Webapp TrackORA untuk melacak pengiriman unit mobil baru ke cabang-cabang. Digunakan oleh orang cabang atau siapa pun yang ingin melacak status unit berdasarkan No. Rangka. Admin (dengan PIN) dapat mengubah status unit.

🧰 Tools yang Digunakan
Tools	Fungsi	Status
GitHub	Repository kode & version control	✅ Aktif
GitHub Pages	Hosting website live & publik	✅ Aktif
Chrome DevTools	Preview responsive (desktop & mobile)	✅ Aktif
GitHub Editor	Editor kode online	✅ Aktif
URL Penting:
Repository: https://github.com/maulinanda/trackora-web

Website Live: https://maulinanda.github.io/trackora-web/

📁 Struktur File Saat Ini
text
trackora-web/
├── README.md
└── index.html        ← Seluruh kode (HTML + CSS + JavaScript dalam 1 file)
Catatan: Semua masih dalam 1 file. Belum dipisah ke CSS/JS eksternal.

🧠 Semua Konsep yang Sudah Dipelajari
HTML
Konsep	Penerapan
Struktur dasar	<!DOCTYPE>, <html>, <head>, <body>
Meta tag	charset, viewport
Heading & Paragraf	<h1> - <h3>, <p>
Div & Span	<div>, <span> untuk grouping
Form Input	<input> text, password, search
Button	<button> dengan onclick
Class & ID	Untuk CSS selector dan JavaScript
Komentar HTML	<!-- ... -->
CSS
Konsep	Penerapan
Selector Elemen, Class, ID	body, .kartu, #errorMsg
Warna	Hex, rgb, rgba, nama warna
Font	font-family, font-size, font-weight, letter-spacing
Box Model	margin, padding, border-radius, border
Flexbox	display: flex, align-items, justify-content, gap
Grid	display: grid, grid-template-columns, repeat, auto-fill
Position	relative, absolute, fixed
Shadow	box-shadow untuk efek mengambang dan glow
Animation	@keyframes pulse, popIn, shake, fadeIn
Pseudo-element	::after untuk garis penghubung progress
Pseudo-class	:hover, :focus, :not(:last-child), :disabled
Media Query	@media (max-width: 600px) untuk responsive mobile
Transition	transition: all 0.3s
Z-index	Untuk overlay/modal
Transform	translateY, scale untuk efek hover
JavaScript
Konsep	Penerapan
Variabel (let, const)	adminMode, unitAktif, filterStatus, daftarUnit
Array	daftarUnit (data unit), statusListNormal, statusListRecon
Object	Setiap unit: { rangka, tujuan, status, perluReconditioning, tanggal }
Array of Objects	Struktur data utama
Fungsi	cekStatus(), renderDashboard(), hitungStats(), setFilter(), dll
Parameter & Return	Semua fungsi menerima dan/atau mengembalikan nilai
Event Listener	Klik, Enter, Escape, input real-time
DOM Manipulation	getElementById(), innerHTML, classList.add/remove/toggle
Kondisional	if/else, switch/case, ternary ? :
Loop	for loop untuk progress bar, for...of untuk stats
Array Methods	.find(), .filter(), .length
String Methods	.trim(), .toLowerCase(), .includes()
Date Object	new Date(), getDate(), getMonth(), getFullYear()
localStorage	setItem(), getItem(), removeItem() — sesi admin 30 menit
setTimeout	Notifikasi hilang otomatis 3 detik
Dynamic CSS via JS	Membuat <style> untuk animasi shake
Grid Dynamic Rendering	Render kartu dashboard dari array data
🔐 Fitur Keamanan
Fitur	Detail
PIN Admin	Default: 1234 (ganti di variabel ADMIN_PIN)
Sesi 30 Menit	Disimpan di localStorage key trackora_admin_sesi
Auto-login	Cek sesi saat halaman dimuat
Popup Login	Overlay gelap, input PIN tersembunyi (type password)
Efek PIN Salah	Popup goyang (animasi shake) + error merah
Escape/Batal	ESC atau klik luar popup untuk batal
📊 Fitur Dashboard
Fitur	Cara Kerja
Stats Bar	5 kartu: Total, DR Created, Preparation, In Transit, Delivered
Klik Filter	Klik stat card → filter unit dengan status itu. Klik lagi → reset
Real-time Search	Ketik No. Rangka → langsung filter kartu
Info Filter	Menampilkan "X dari Y unit" saat filter aktif
Reset Button	Muncul saat filter/search aktif
Empty State	Tampilan khusus saat tidak ada unit yang cocok
Klik Kartu	Klik kartu unit → pindah ke tab Lacak & tampilkan detail
📋 Semua Fitur
Fitur	Status	Keterangan
Tampilan detail unit	✅	No. Rangka + Tujuan
Progress bar dinamis	✅	4 atau 5 tahap sesuai kondisi
Quality Reconditioning	✅	Status opsional, toggle ON/OFF
Animasi status aktif	✅	Efek pulsing
Garis penghubung step	✅	Hijau/oranye/abu sesuai status
Responsive mobile	✅	Media query < 600px
Input cari No. Rangka	✅	Enter atau klik tombol
Error handling	✅	Input kosong / tidak ditemukan
Dashboard semua unit	✅	Grid kartu responsif
Stats bar + counter	✅	5 kartu statistik
Search dashboard	✅	Real-time filter
Filter by status	✅	Klik stat card
Panel Admin	✅	Ubah status unit
Toggle Reconditioning	✅	Admin bisa ON/OFF per unit
Login Admin PIN	✅	Popup + localStorage sesi
Notifikasi	✅	Muncul 3 detik, auto-hilang
Tambah unit baru	❌	Data dari database, bukan manual
Backend/Database	❌	Masih data dummy di JavaScript
🚗 Data Dummy
No. Rangka	Tujuan	Status	Reconditioning
MHFAB1CJ2N1234567	Cabang Jakarta Pusat	In Transit	✨ Ya
MHFAB1CJ2N7654321	Cabang Bandung	Unit Preparation	❌ Tidak
MHFAB1CJ2N9999999	Cabang Surabaya	Delivered	✨ Ya
🔜 Rencana Selanjutnya
Fase Backend (Database Nyata)
Pemisahan File — CSS ke style.css, JS ke script.js

Node.js + Express — Server backend

Database — JSON file / SQLite / PostgreSQL

API REST — Endpoint untuk baca & update status

Fetch API — JavaScript panggil data dari server

Deploy Backend — Railway / Render / Vercel (gratis)

💡 Cara Mengganti PIN Admin
Di bagian <script>, cari baris:

javascript
const ADMIN_PIN = "1234";
Ubah angkanya, commit, refresh.

💡 Cara Melanjutkan di Chat Baru
Copy-paste checkpoint ini dan kirim ke chat baru bersama pesan:

"Saya sedang membangun project TrackORA Web untuk logistik mobil. Ini checkpoint #3. Saya ingin melanjutkan ke [fase backend / pemisahan file / fitur lain]."
