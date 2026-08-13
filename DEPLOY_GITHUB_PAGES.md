# Deploy ke GitHub Pages

1. Buat repository baru di GitHub, misalnya `framinglab-scientific`.
2. Unggah **seluruh isi folder ini** ke root repository:
   - `index.html`
   - `style.css`
   - `app.js`
   - `.nojekyll`
   - `README.md`
   - `CITATION.cff`
   - `VERSION.txt`
3. Buka **Settings → Pages**.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch **main** dan folder **/(root)**.
6. Klik **Save**.
7. Tunggu proses deploy. Situs akan tersedia pada alamat `https://USERNAME.github.io/NAMA-REPOSITORY/`.

Aplikasi tidak membutuhkan backend. Akses ke Crossref, DataCite, Open Library, GDELT, Jina Reader, dan OpenAlex bergantung pada ketersediaan layanan eksternal dan kebijakan CORS masing-masing saat aplikasi digunakan.
