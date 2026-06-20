📦 CHECKPOINT #4 — TrackORA Web
Tanggal: 20 Juni 2026
Status Project: Frontend lengkap pasca iterasi besar. Fitur stabil, tampilan sesuai kebutuhan logistik mobil. Siap masuk fase backend/database.

🎯 Tujuan Project
Webapp TrackORA untuk melacak pengiriman unit mobil baru dari pusat distribusi ke cabang-cabang via RVDC Ngoro. Pengguna (orang cabang) melacak status unit berdasarkan No. Rangka. Admin (dengan PIN) dapat mengubah status dan mengelola Quality Reconditioning.

🧰 Tools & URL
Tools	Fungsi
GitHub	Repository & version control
GitHub Pages	Hosting live & publik
Repo: https://github.com/maulinanda/trackora-web

Live: https://maulinanda.github.io/trackora-web/

📁 Struktur File
text
trackora-web/
├── README.md
└── index.html        ← HTML + CSS + JS dalam 1 file
📋 Fitur yang Sudah Jadi
Fitur	Status
🔍 Lacak unit by No. Rangka	✅
📋 Progress bar 4 tahap (DR Created → Unit Preparation → In Transit → Delivered)	✅
🔧 Quality Reconditioning sebagai sub-proses Unit Preparation	✅
🚛 Banner RVDC Ngoro (jika unit masih dalam perjalanan ke RVDC)	✅
📊 Dashboard daftar unit model tabel	✅
🏢 Filter by cabang (dropdown, wajib pilih dulu)	✅
🔐 Login Admin dengan PIN	✅
💾 Sesi admin 30 menit (localStorage)	✅
🛠️ Panel Admin (maju/reset status, toggle QR)	✅
⏰ Semua tanggal tanpa jam (hanya tanggal)	✅
📅 Info detail: No. Rangka, Tujuan, Estimasi Kirim	✅
🚛 Progress In Transit menampilkan Estimasi Tiba	✅
✨ QR menampilkan estimasi selesai rekondisi	✅
📱 Responsive mobile	✅
🎨 Animasi & UX (pulse, popup, shake, notifikasi)	✅
🚗 Data Dummy
No. Rangka	Tujuan	Status	QR?	RVDC?
MHFAB1CJ2N1234567	Cabang Jakarta Pusat	In Transit (3)	❌	❌
MHFAB1CJ2N7654321	Cabang Bandung	Unit Preparation (2)	✨ Ya	🚛 Ya
MHFAB1CJ2N9999999	Cabang Surabaya	Delivered (4)	❌	❌
🧠 Konsep yang Sudah Dipelajari
HTML, CSS, JavaScript
Semua konsep dari Checkpoint #1-#3

Tabel HTML (dashboard list)

Dropdown filter & event onchange

Dynamic option generation (populate cabang)

Date manipulation (H+2 untuk estimasi QR)

Conditional rendering (QR, RVDC, filter wajib)

🔜 Fase Selanjutnya: Backend & Database
Pisah file — CSS & JS ke file terpisah

Node.js + Express — Server backend

Database — JSON file / SQLite / PostgreSQL

API REST — Endpoint: GET unit, PUT update status

Fetch API — Ganti data hardcode dengan fetch()

Deploy Backend — Railway / Render (gratis)

💡 Cara Melanjutkan di Chat Baru
Copy-paste checkpoint ini ke chat baru:

"Saya sedang membangun project TrackORA Web. Ini checkpoint #4. Saya ingin melanjutkan ke fase backend."
