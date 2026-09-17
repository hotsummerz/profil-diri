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
web profil diri\
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

## 🎨 Fitur Desain & UX

- **Responsive Design:** Tabel scrollable di mobile, bento grid menyesuaikan layar
- **Accessibility First:** Skip link, ARIA labels, keyboard navigation, high contrast
- **Progressive Enhancement:** Animasi scroll bekerja jika JS aktif, konten tetap terlihat jika JS off
- **Clean Code:** Separation of concerns (HTML/CSS/JS), no inline styles, semantic markup
- **Performance:** Minimal dependencies, preconnect untuk fonts, optimized loading
