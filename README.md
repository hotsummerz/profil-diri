# Tugas: Membuat Halaman Profil Diri dengan HTML5
**Mata Kuliah:** Pengembangan Aplikasi Web (Semester 5)  
**Program Studi:** S1 Teknik Informatika  
**Tema Desain:** Clean Minimalist UI (FEARNOT Blue • Pantone 7453 C)

---

## 📋 Ringkasan Penilaian & Pemenuhan Kriteria (100%)

Proyek ini telah dikembangkan dengan mematuhi seluruh spesifikasi tugas dan standar penulisan kode modern:

| Kriteria Penilaian | Bobot | Status | Detail Implementasi |
| :--- | :---: | :---: | :--- |
| **1. Struktur HTML5** | 25% | ✅ Terpenuhi Penuh | Memakai `<!DOCTYPE html>`, `<html lang="id">`, serta elemen semantik `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<figcaption>`, `<address>`, `<time>`, dan `<footer>`. |
| **2. Aksesibilitas (A11y)** | 25% | ✅ Terpenuhi Penuh | Meliputi *skip link* (`.skip-link`), teks alternatif (`alt`) deskriptif pada foto, atribut `scope="col"` & `scope="row"` pada tabel, rasio kontras WCAG 2.1 AAA, dan *focus ring* yang jelas untuk navigasi keyboard. |
| **3. Metadata Lengkap** | 25% | ✅ Terpenuhi Penuh | Menyertakan `<title>`, `<meta name="description">`, Open Graph lengkap (`og:title`, `og:description`, `og:image`, `og:type`), `<meta name="viewport">`, dan karakter set UTF-8. |
| **4. Kerapihan Kode** | 25% | ✅ Terpenuhi Penuh | Indentasi konsisten 2-spasi, pemisahan berkas antara struktur (`index.html`) dan presentasi (`style.css`), serta komentar penjelas yang rapi dan terstruktur. |

---

## 🗂️ Struktur Direktori Proyek

```text
D:\IF\Tugas\Sem 5\pengembangan aplikasi web\web profil diri\
├── index.html            # Berkas utama halaman profil diri HTML5 semantik
├── style.css             # Berkas CSS styling bertema Clean Minimalist
├── script.js             # JavaScript untuk scroll reveal animation
├── README.md             # Dokumentasi tugas dan checklist penilaian
└── assets/
    └── images/
        ├── avatar.svg    # Foto/vektor potret profil diri (scalable & tajam)
        └── og-image.svg  # Gambar banner untuk metadata Open Graph (social share)
```

---

## 🔍 Rincian Fitur & Pemenuhan Ketentuan Tugas

### 1. Hierarki Heading yang Benar
- **`<h1>`**: Judul nama utama mahasiswa.
- **`<h2>`**: Judul seksi utama (*Biodata Diri*, *Mata Kuliah Semester Ini*, *Kontak & Tautan Terkait*).
- **`<h3>`**: Sub-judul dalam kartu bento (*Identitas Akademik Mahasiswa*, *Fokus Peminatan*, *Tentang Saya*).
- *Tidak ada loncatan level heading* (selalu berurutan h1 → h2 → h3).

### 2. Foto Diri dengan Atribut `alt`
- Disematkan menggunakan tag semantik `<figure>` dan `<figcaption>`.
- Dilengkapi atribut `alt` yang deskriptif.
- Dilengkapi atribut `loading="eager"` untuk prioritas loading.

### 3. Tabel Mata Kuliah Semester 5
- Menggunakan elemen tabel HTML5 lengkap: `<table>`, `<thead>`, `<tbody>`.
- Aksesibilitas kolom menggunakan `scope="col"` dan `scope="row"`.
- Daftar 7 mata kuliah semester 5 dengan total **20 SKS**.
- Kolom: No., Nama Mata Kuliah, SKS, Jadwal Kuliah, Kelas.
- Dilengkapi wadah pembungkus responsif dengan `tabindex="0"` dan `role="region"` agar ramah keyboard.

### 4. Tautan (Link)
- **Tautan Internal Navigasi:** Loncat antar-seksi (`#tentang`, `#biodata`, `#matakuliah`, `#kontak`).
- **Tautan Eksternal:** GitHub, LinkedIn, dan tautan `mailto:` email dengan atribut keamanan `target="_blank"` dan `rel="noopener noreferrer"`.

### 5. Metadata & Open Graph
- `<title>`: Judul resmi dokumen yang informatif.
- `<meta name="description">`: Deskripsi singkat ringkasan halaman.
- `<meta property="og:title">`: Judul saat dibagikan ke media sosial.
- `<meta property="og:description">`: Deskripsi ringkas saat tautan dibagikan.
- `<meta property="og:image">`: Gambar banner (`og-image.svg`).

### 6. Typography & Styling
- Font utama: **Geist** (sans-serif modern & clean)
- Font monospace: **Geist Mono** untuk kode & badge
- Navigasi centered di header, footer centered
- Inline styles dipindah ke CSS untuk maintainability
- Scroll reveal animation menggunakan IntersectionObserver (progressive enhancement)

---

## 💡 Panduan Kustomisasi Data Pribadi

Bila ingin menyesuaikan data profil dengan identitas Anda:
1. Buka `index.html` menggunakan teks editor (VS Code, Notepad++, dll).
2. Ubah teks **Nama**, **NIM**, **Universitas**, serta daftar mata kuliah sesuai jadwal Anda.
3. **Mengganti Foto:** Letakkan file foto Anda (misalnya `foto-saya.jpg`) ke dalam folder `assets/images/`, lalu ganti atribut `src="assets/images/avatar.svg"` menjadi `src="assets/images/foto-saya.jpg`.

---

## 🎨 Fitur Desain & UX

- **Responsive Design:** Tabel scrollable di mobile, bento grid menyesuaikan layar
- **Accessibility First:** Skip link, ARIA labels, keyboard navigation, high contrast
- **Progressive Enhancement:** Animasi scroll bekerja jika JS aktif, konten tetap terlihat jika JS off
- **Clean Code:** Separation of concerns (HTML/CSS/JS), no inline styles, semantic markup
- **Performance:** Minimal dependencies, preconnect untuk fonts, optimized loading
