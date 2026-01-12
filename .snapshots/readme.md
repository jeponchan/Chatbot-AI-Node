
# Chatbot AI Node

Chatbot web sederhana menggunakan Node.js, Express, EJS dan API AI (misalnya OpenAI/ChatGPT). Aplikasi ini menyediakan UI chat di browser dan mengirim pesan ke model AI melalui endpoint backend.

## Fitur

- UI chat sederhana di browser.
- Komunikasi dua arah (user ↔ bot).
- Pesan dikirim ke API AI dan ditampilkan kembali sebagai balasan.
- Arsitektur dipisah antara frontend (EJS + JS) dan backend (Express + API AI), mengikuti pola umum integrasi Node + OpenAI.

## Teknologi

- Node.js
- Express.js
- EJS
- Fetch API (AJAX) di frontend
- openai (client resmi untuk API OpenAI / model kompatibel)

## Persiapan Lingkungan

1. Pastikan sudah terpasang:
   - Node.js (LTS)
2. Clone repository:

   git clone https://github.com/jeponchan/Chatbot-AI-Node.git
   cd chatbot-ai-node
3. Install dependency:

    npm install
4. Buat file .env di root proyek:

OPENAI_API_KEY=ISI_API_KEY_ANDA
PORT=4000

## Menjalankan Aplikasi

npm start

Lalu buka di browser:

http://localhost:4000

Cara Menggunakan
1. Buka halaman utama:

    Akan tampil kotak chat dengan area percakapan dan input pesan.

2. Ketik pesan di kolom input, lalu tekan Kirim.

3. Pesan akan:

    - Ditampilkan sebagai pesan user.

    - Dikirim ke endpoint /api/chat di backend.

    - Backend akan memanggil API AI menggunakan library openai dan mengirim balasan.

    - Balasan akan tampil di area chat sebagai pesan bot.