# Tallysheet Gambut Backend

Sistem backend untuk pengolahan formulir Tallysheet Gambut berbasis Node.js + Express.

## Fitur

* Menerima data formulir dari frontend.
* Menerima upload gambar sketsa lokasi dan foto lapangan.
* Menghasilkan output file Word (DOCX) sesuai dengan template Tallysheet - Gambut\_2.docx.

## Teknologi

* Node.js + Express
* Multer
* Docxtemplater + PizZip
* UUID

## Struktur File Utama

* `index.js` → File utama backend.
* `template/Tallysheet - Gambut_2.docx` → Template form Word.
* `package.json` → Konfigurasi dependency dan script.

## Cara Menjalankan Lokal

1. Clone repository:

```bash
https://github.com/Sarxean/tallysheet-gambut-backend.git
```

2. Install dependency:

```bash
npm install
```

3. Jalankan server:

```bash
npm start
```

Server berjalan di `http://localhost:3001`.

## Endpoint API

POST `/api/generate-tallysheet`

* Body: `multipart/form-data`
* Field input sesuai dengan FormTallysheet dari frontend.

## Catatan

* Pastikan file template `.docx` sudah diletakkan di folder `/template`.
* Untuk pengolahan gambar di dalam DOCX, dapat menggunakan image-module tambahan jika diperlukan.

---

Jika membutuhkan panduan deploy ke Replit atau Vercel, silakan lihat dokumentasi tambahan.
