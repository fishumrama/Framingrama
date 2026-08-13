# Deploy FramingLab ke GitHub Pages

## Opsi antarmuka GitHub

1. Masuk ke GitHub dan pilih **New repository**.
2. Nama repository yang disarankan: `framinglab-web-research`.
3. Pilih **Public** atau **Private** sesuai akun dan kebijakan GitHub Pages Anda.
4. Upload file berikut ke root repository:
   - `index.html`
   - `style.css`
   - `app.js`
   - `README.md`
   - `.nojekyll`
   - `CITATION.cff`
5. Commit ke branch `main`.
6. Buka **Settings → Pages**.
7. Pilih **Deploy from a branch** → `main` → `/(root)` → **Save**.
8. Tunggu proses deploy selesai.

## Opsi Git CLI

```bash
git init
git add .
git commit -m "FramingLab Web Research Edition v5"
git branch -M main
git remote add origin https://github.com/USERNAME/framinglab-web-research.git
git push -u origin main
```

Kemudian aktifkan GitHub Pages dari **Settings → Pages**.

## Mengapa versi ini compatible dengan GitHub Pages?

Versi lama memakai Python/FastAPI (`/api/analyze`) sehingga membutuhkan server aplikasi. Versi v5 memindahkan analisis teori ke JavaScript di browser dan menggunakan API publik melalui HTTPS. Semua path aset memakai path relatif (`./style.css`, `./app.js`).
