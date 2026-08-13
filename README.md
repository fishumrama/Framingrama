# FramingLab by Rama Kertamukti — Scientific Narrative Edition v6.0

FramingLab adalah aplikasi analisis framing berita berbasis browser yang dapat dipublikasikan sebagai situs statis melalui GitHub Pages.

## Pembaruan v6

- Mendeteksi dan menolak halaman CAPTCHA, security verification, access denied, dan halaman non-artikel sebelum dianalisis.
- Menghasilkan interpretasi **naratif** untuk Entman, Pan & Kosicki, Gamson & Modigliani, dan Edelman.
- Memisahkan bukti teks primer dari interpretasi teori.
- Menelusuri metadata jurnal/karya ilmiah melalui Crossref dan DataCite.
- Menelusuri buku/monograf melalui Open Library.
- Mendukung OpenAlex secara opsional menggunakan API key pengguna.
- Menyediakan kolom catatan ilmiah peneliti yang tidak dicampur dengan hasil web.
- Membuat **Sintesis Ilmiah** dari metadata/abstrak yang benar-benar tersedia tanpa mengarang temuan artikel.
- Triangulasi berita pembanding melalui GDELT.
- Ekspor TXT, HTML, dan JSON.

## Menjalankan

Cukup buka `index.html` atau publikasikan repository melalui GitHub Pages. Tidak diperlukan Python, FastAPI, Node.js, atau database.

## Prinsip integritas

Aplikasi tidak menganggap metadata bibliografis sebagai bukti isi artikel. Bila abstrak tidak tersedia, hasil hanya ditampilkan sebagai metadata dan pengguna diminta membaca teks penuh sebelum mengutip temuan. CAPTCHA/security page tidak dianalisis sebagai berita.

## Deploy GitHub Pages

Lihat `DEPLOY_GITHUB_PAGES.md`.

Powered by Rama Kertamukti Media dan Komunikasi UIN Sunan Kalijaga Yogyakarta.
