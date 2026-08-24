# ☁️ Portofolio Cloud Computing — [Nama Anda]

Portofolio pribadi berbasis **HTML & CSS murni** (tanpa framework) untuk menampilkan profil, keahlian, proyek, dan sertifikasi sebagai lulusan Cloud Computing. Website ini dirancang agar bisa langsung di-deploy gratis menggunakan **GitHub Pages**.

🔗 **Live Demo:** `https://<username-github-anda>.github.io/<nama-repo>/`
> Ganti link di atas setelah kamu selesai deploy (lihat langkah 4 di bawah).

---

## 📁 Struktur File

```
portfolio/
├── index.html   # Seluruh halaman (HTML + CSS + sedikit animasi) dalam satu file
└── README.md    # Dokumentasi ini
```

---

## ✏️ Cara Kustomisasi

Sebelum deploy, buka `index.html` lalu ganti bagian berikut sesuai data kamu:

| Bagian | Cari teks | Ganti dengan |
|---|---|---|
| Judul tab & logo | `Nama Anda`, `nama-anda.dev` | Nama kamu |
| Hero / perkenalan | `[Nama Anda]` | Nama lengkap kamu |
| Tombol CV | `href="#"` pada tombol *Unduh CV* | Link file CV kamu (Google Drive/PDF) |
| Tentang Saya | Paragraf di bawah `<section id="about">` | Ceritakan latar belakang kamu |
| Keahlian | Isi `<div class="tag-row">` | Sesuaikan tools/skill yang kamu kuasai |
| Proyek | Setiap `<div class="project-card">` | Judul, deskripsi, dan link repo/demo proyekmu |
| Sertifikasi | Setiap `<div class="cert-pill">` | Nama sertifikasi yang kamu punya |
| Kontak | `mailto:email.anda@example.com`, link LinkedIn & GitHub | Data kontak kamu |

Tidak perlu tools tambahan — cukup edit dengan text editor apa pun (VS Code, Notepad, dll), lalu buka `index.html` di browser untuk melihat hasilnya secara lokal.

---

## 🚀 Langkah Deploy ke GitHub Pages

### 1. Buat repository baru di GitHub
- Login ke [github.com](https://github.com)
- Klik **New repository**
- Beri nama, misalnya `portfolio` atau `username-anda.github.io`
- Set ke **Public**, lalu klik **Create repository**

### 2. Upload file ke repository
**Opsi A — lewat web (tanpa command line):**
- Di halaman repo, klik **Add file → Upload files**
- Seret file `index.html` dan `README.md`, lalu klik **Commit changes**

**Opsi B — lewat Git/terminal:**
```bash
git init
git add index.html README.md
git commit -m "Initial commit: portofolio cloud computing"
git branch -M main
git remote add origin https://github.com/<username-anda>/<nama-repo>.git
git push -u origin main
```

### 3. Aktifkan GitHub Pages
- Buka repo → tab **Settings**
- Di sidebar kiri, klik **Pages**
- Pada **Source**, pilih branch **main** dan folder **/(root)**
- Klik **Save**

### 4. Ambil link portofolio kamu
- Tunggu 1–2 menit, GitHub akan menampilkan link berbentuk:
  ```
  https://<username-anda>.github.io/<nama-repo>/
  ```
- Jika nama repo kamu adalah `username-anda.github.io`, link-nya langsung menjadi:
  ```
  https://<username-anda>.github.io/
  ```
- Buka link tersebut untuk memastikan portofolio sudah tampil online, lalu update bagian **Live Demo** di README ini dengan link tersebut.

### 5. (Opsional) Custom domain
Jika punya domain sendiri, tambahkan file `CNAME` berisi nama domain, lalu atur DNS record (CNAME) mengarah ke `<username-anda>.github.io`. Pengaturan lengkap ada di menu **Settings → Pages → Custom domain**.

---

## 🛠️ Tech Stack
- HTML5 & CSS3 (tanpa framework/build tool)
- Google Fonts: *Space Grotesk*, *Inter*, *JetBrains Mono*
- SVG untuk diagram arsitektur sederhana
- Hosting: GitHub Pages (gratis)

---

## 📄 Lisensi
Bebas digunakan dan dimodifikasi untuk keperluan portofolio pribadi.
