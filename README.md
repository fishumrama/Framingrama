# FramingLab by Rama Kertamukti — Web Research Edition v5.0

Aplikasi analisis framing berita yang berjalan sebagai **static web app** dan siap dipublikasikan melalui **GitHub Pages**. Tidak memerlukan FastAPI, Python server, database, atau build process.

## Fitur utama

- Model Robert N. Entman.
- Model Pan & Kosicki.
- Model Gamson & Modigliani.
- Model Murray Edelman.
- Interpretasi sederhana: inti frame, aktor/entitas menonjol, istilah utama, pola sebab, arah moral, dan catatan kehati-hatian.
- Kolom fokus/pertanyaan penelitian untuk membuat analisis dan pencarian lebih terarah.
- Membaca URL melalui **Jina Reader** tanpa API key untuk penggunaan dasar; teks manual tetap disediakan sebagai fallback.
- Pencarian otomatis berita pembanding melalui **GDELT DOC API**.
- Pencarian metadata literatur ilmiah melalui **Crossref REST API**.
- Pencarian DOI/repository metadata melalui **DataCite Public REST API**.
- Tidak membuat referensi, DOI, kutipan, atau fakta baru yang tidak dikembalikan sumber.
- Ekspor laporan TXT, HTML, dan JSON.
- Responsive dan compatible dengan GitHub Pages.

## Cara menjalankan lokal

Cukup buka `index.html` di browser. Untuk pengujian yang paling mirip GitHub Pages, jalankan server statis sederhana, misalnya:

```bash
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Deploy GitHub Pages

1. Buat repository GitHub baru, misalnya `framinglab`.
2. Upload seluruh isi folder ini ke branch `main`.
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch **main** dan folder **/(root)**.
6. Klik **Save**.

Alamat publik akan berbentuk:

`https://USERNAME.github.io/framinglab/`

## Catatan metodologis

FramingLab adalah alat bantu coding dan interpretasi awal. Hasil tidak menggantikan pembacaan kualitatif peneliti. Daftar berita pembanding dan literatur ilmiah adalah hasil retrieval metadata/pencarian; keberadaannya tidak otomatis membuktikan atau membantah isi berita utama. Peneliti tetap perlu membaca sumber asli dan, untuk artikel ilmiah, teks penuh sebelum menyimpulkan temuan penelitian.

## Sumber web eksternal

Aplikasi menggunakan endpoint publik pihak ketiga. Ketersediaan, pembatasan kuota, CORS, dan kebijakan layanan dapat berubah. Jika satu layanan gagal, analisis framing lokal tetap dapat berjalan dan aplikasi menampilkan catatan kegagalan tersebut.

## Kredit

**Powered by Rama Kertamukti Media dan Komunikasi UIN Sunan Kalijaga Yogyakarta**
