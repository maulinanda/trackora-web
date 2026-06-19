📦 CHECKPOINT #2 — TrackORA Web
Tanggal: 20 Juni 2026
Status Project: Webapp interaktif dengan sistem login admin, siap untuk fitur lanjutan

🎯 Tujuan Project
Webapp TrackORA untuk melacak pengiriman unit mobil baru ke cabang-cabang. Pengguna (orang cabang/siapa pun) bisa melacak status unit berdasarkan No. Rangka. Admin bisa mengubah status unit melalui Panel Admin dengan PIN.

🧰 Tools yang Digunakan
Tools	Fungsi	Status
GitHub	Repository kode & version control	✅ Aktif
GitHub Pages	Hosting website live & publik	✅ Aktif
Chrome DevTools	Preview responsive (desktop & mobile)	✅ Aktif
GitHub Editor / vscode.dev	Editor kode online	✅ Aktif
URL Penting:
Repository: https://github.com/maulinanda/trackora-web

Website Live: https://maulinanda.github.io/trackora-web/

📁 Struktur File
text
trackora-web/
├── README.md
└── index.html        ← Seluruh kode (HTML + CSS + JavaScript)
Catatan: Masih satu file. Belum ada pemisahan CSS/JS eksternal.

🧠 Konsep yang Sudah Dipelajari
HTML
Konsep	Penerapan
Struktur dasar	<!DOCTYPE>, <html>, <head>, <body>
Meta tag	charset, viewport untuk responsive
Heading	<h1> - <h3>
Paragraf	<p>
Div/Span	<div>, <span> untuk grouping
Form input	<input> text & password
Button	<button> dengan atribut onclick
Class	Label untuk CSS selector
Komentar HTML	<!-- ... -->
CSS
Konsep	Penerapan
Selector Elemen	body, h1, h2, p
Selector Class	.kartu, .indikator-selesai
Warna	Hex #2e7d32, rgb rgba(0,0,0,0.5)
Font	font-family, font-size, font-weight, letter-spacing
Box Model	margin, padding, border-radius
Flexbox	display: flex, align-items, justify-content
Position	position: relative/absolute/fixed
Shadow	box-shadow untuk efek mengambang
Animation	@keyframes pulse, @keyframes popIn, @keyframes shake
Pseudo-element	::after untuk garis penghubung
Pseudo-class	:hover, :focus, :not(:last-child)
Media Query	@media (max-width: 480px) untuk responsive mobile
Transition	transition: all 0.3s
Z-index	z-index untuk overlay
Overlay/Modal	Latar gelap + popup di tengah
JavaScript
Konsep	Penerapan
Variabel (let, const)	adminMode, unitAktif, daftarUnit, ADMIN_PIN
Array	daftarUnit (kumpulan 3 unit), statusList (4 tahap)
Object	Setiap unit: { rangka, tujuan, status, tanggal }
Fungsi	cekStatus(), tampilkanProgress(), majuStatus(), dll
Parameter & Return	tampilkanProgress(unit), dapatkanDetailStatus(unit, index)
Event Listener	Klik tombol, Enter di input, Escape, klik overlay
DOM Manipulation	getElementById(), innerHTML, classList.add/remove
Kondisional	if/else, switch/case, ternary
Loop	for loop untuk menggambar 4 step progress
Array.find()	Mencari unit berdasarkan No. Rangka
String methods	.trim(), .toLowerCase()
Date object	new Date() untuk tanggal otomatis
localStorage	setItem(), getItem(), removeItem() untuk sesi admin
setTimeout	Notifikasi hilang otomatis 3 detik
CSS via JS	Membuat <style> dinamis untuk animasi shake
🔐 Fitur Keamanan
Fitur	Detail
PIN Admin	Default: 1234 (bisa diganti di variabel ADMIN_PIN)
Sesi 30 Menit	Disimpan di localStorage dengan key trackora_admin_sesi
Auto-login	Cek sesi saat halaman dimuat
Popup Login	Overlay gelap, input PIN tersembunyi (type password)
Efek PIN Salah	Popup goyang + error merah
Logout	Tombol keluar + hapus sesi
📋 Status Fitur
Fitur	Status	Keterangan
Tampilan detail unit	✅ Selesai	No. Rangka + Tujuan
Progress bar 4 tahap	✅ Selesai	Indikator warna & animasi pulsing
Animasi status aktif	✅ Selesai	Efek pulsing pada status saat ini
Garis penghubung step	✅ Selesai	Hijau (selesai), abu (belum)
Responsive mobile	✅ Selesai	Media query untuk layar < 480px
Input cari No. Rangka	✅ Selesai	Bisa Enter atau klik tombol
Error handling	✅ Selesai	Pesan jika kosong / tidak ditemukan
Data dummy 3 unit	✅ Selesai	3 No. Rangka dengan status berbeda
Panel Admin	✅ Selesai	Ubah status unit
Login Admin PIN	✅ Selesai	Popup + localStorage sesi
Notifikasi	✅ Selesai	Muncul 3 detik lalu hilang
Status opsional	⏳ Siap	"Quality Reconditioning" sudah diketik, tinggal un-comment
Dashboard multi-unit	❌ Belum	-
Tambah unit baru	❌ Belum	-
Backend/Database	❌ Belum	Masih data dummy di JavaScript
🚗 Data Dummy
No. Rangka	Tujuan	Status
MHFAB1CJ2N1234567	Cabang Jakarta Pusat	In Transit (3)
MHFAB1CJ2N7654321	Cabang Bandung	Unit Preparation (2)
MHFAB1CJ2N9999999	Cabang Surabaya	Delivered (4)
🔜 Rencana Fitur Selanjutnya
Dashboard Multi-Unit — Lihat semua unit sekaligus

Status "Quality Reconditioning" Dinamis — Status opsional yang bisa muncul

Form Tambah Unit Baru — Admin bisa menambah unit

Pemisahan File — CSS & JS dipisah ke file terpisah

Backend dengan Node.js — Database sungguhan, API

💡 Cara Mengganti PIN Admin
Di bagian <script>, cari baris:

javascript
const ADMIN_PIN = "1234";        // Ganti PIN di sini kalau perlu
Ubah "1234" jadi PIN pilihanmu. Commit dan refresh halaman.

💡 Cara Melanjutkan di Chat Baru
Copy-paste checkpoint ini dan kirim ke chat baru bersama pesan:

"Saya sedang membangun project TrackORA Web untuk logistik mobil. Ini checkpoint #2. Saya ingin melanjutkan dari [sebutkan fitur yang diinginkan]."
