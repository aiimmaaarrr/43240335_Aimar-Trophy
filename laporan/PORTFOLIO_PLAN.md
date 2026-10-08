# 🚀 Aimar Trophy Sudrajat — Portfolio Project Plan & Specifications

Dokumen ini merupakan panduan dan cetak biru (*Master Plan*) dalam membangun web portofolio interaktif berbasis *Data Operations & Business Intelligence* milik Aimar Trophy Sudrajat.

---

## 1. Ringkasan Proyek & Tech Stack
- **Jenis Web:** Single-page Landing Page Portfolio (Data Analyst & BI Specialist).
- **Tech Stack:**
  - **HTML5:** Struktur semantik, aksesibilitas tinggi, & SEO-friendly.
  - **CSS3:** Vanilla CSS dengan struktur *Clean Paper Lines & Data Grid*, *Glassmorphism*, kustom properti (`:root`), serta animasi *micro-tilt* pada badge keahlian.
  - **JavaScript:** Vanilla JS (ES6+) untuk interaktivitas dinamis (navigasi responsif, *smooth scrolling*, indikator tautan aktif, dan efek interaksi kartu).
  - **Typography:** Perpaduan Google Fonts *Plus Jakarta Sans* (Heading), *Inter* (Body), dan *JetBrains Mono* (Metrics & Monospace badges).
  - **Deployment:** Vercel Ready (`aimartrophysudrajat-portfolio.vercel.app`).
- **Tema & Style:** *Tactile Analyst & Midnight Telemetry* (kombinasi warna gelap elegan khas data terminal, aksen *Emerald Green* serta *Data Amber/Yellow*, dipadu garis kertas kerja yang rapi).

---

## 2. Variabel Desain & Sistem Warna (Design Tokens)
Definisi variabel CSS kustom yang merepresentasikan identitas visual portofolio:

```css
:root {
  /* Color Palette - Tactile Analyst / Midnight Telemetry */
  --bg-primary: #0B0E14;        /* Midnight Dark (Background utama) */
  --bg-card: #131313;           /* Deep Slate Card (Container & kartu) */
  --accent-primary: #05636B;    /* Tactile Blue (Aksen utama korporat) */
  --accent-emerald: #06D2A8;    /* Emerald Green (Status & badge aktif) */
  --accent-amber: #FFD036;      /* Data Amber/Yellow (Highlight & kompetisi) */
  --text-primary: #F8FAFC;      /* Teks Utama (Heading & teks tebal) */
  --text-secondary: #94A3B8;    /* Teks Sekunder (Paragraf & deskripsi) */

  /* Typography */
  --font-heading: 'Plus Jakarta Sans', sans-serif;
  --font-body: 'Inter', sans-serif;
  --font-mono: 'JetBrains Mono', monospace;

  /* UI Accents & Glass */
  --border-color: rgba(255, 255, 255, 0.1);
  --glass-bg: rgba(19, 19, 19, 0.85);
  --shadow-glow: 0 0 20px rgba(6, 210, 168, 0.15);
}

## 3. Struktur Navigasi (Navbar)
Navbar melayang (*Fixed/Sticky*) dengan efek *glassmorphism* dan menu adaptif:
1. Home (`#home`)
2. About (`#about`)
3. Experience (`#experience`)
4. Skills (`#skills`)
5. Projects (`#projects`)
6. Contact (`#contact`)

---

## 4. Detail Struktur Halaman & Konten (Single-Page Application)

### 📍 Header / Navbar
- **Brand / Logo:** *AT.* (`aimartrophy.data` dengan sub-label *data operations & bi*).
- **Menu Navigasi Desktop & Mobile:** 5 tautan utama, tombol pengalih tema/bahasa, serta tombol interaktif *"Contact Me"*.
- **Efek Interaktif:** *Backdrop Blur* saat halaman discroll.

### 📍 Section 1: Home / Hero Section
- **Badge Status:** *"OPEN TO DATA ANALYTICS & BI ROLES"* (ready for fulltime/contract).
- **Headline:** Nama lengkap dengan aksen blok warna kuning (*Aimar Trophy Sudrajat*).
- **Sub-headline & Status Akademik:** *Data Analyst & Information Systems Student* di STMIK IKMI Cirebon.
- **Value Proposition:** Narasi pengolahan data mentah menjadi *actionable business intelligence* dan *visual story* yang didukung pengalaman operasional korporat nyata.
- **Key Stats Badges:** Menyoroti pencapaian (misal: Penghargaan Data Viz Nasional, Audit Presisi Tinggi, dll).
- **Call-to-Action (CTA):** Tombol *Explore Featured Projects* & *Get in Touch*.

### 📍 Section 2: About & Academic Rigor (Background & Timeline)
- **Latar Belakang:** Perpaduan unik antara pengalaman operasional korporat/finansial (sebelum kuliah) dan keilmuan sistem informasi akademis.
- **Sub-section Education:** Detail status kuliah di STMIK IKMI Cirebon (NIM 43240335, Semester berjalan, fokus pada basis data relasional & pemodelan keputusan).

### 📍 Section 3: Experience & Professional Background
- **Timeline Pengalaman Nyata:** 
  - Pengalaman kerja profesional sebagai pengawas/vault teller dan operasional industri (PT Prosegur Cash Indonesia, PT Indo Sultan Jaya, PT Tera Data Indonusa).
  - Penekanan pada akurasi tinggi, kepatuhan prosedur (*compliance*), dan penanganan data fisik/digital bervolume tinggi.

### 📍 Section 4: Data Stack & Technical Matrix (Skills & Competencies)
- **Kategori Utama (dengan efek *micro-tilt* saat di-hover):**
  - **Analytics & BI:** Tableau Public, Python (Pandas, NumPy, Seaborn), SQL & Databases (MySQL, PostgreSQL, Joins), Advanced Excel (PowerQuery, Pivot, XLOOKUP).
  - **Data Science & Modeling:** RapidMiner, R Language, Data Cleansing & Missing Data Imputation.
  - **Systems & Automation:** n8n Automation, Laravel & PHP, Figma & Wireframing.

### 📍 Section 5: Projects Showcase
- **Grid Proyek Unggulan:** Menampilkan proyek riwayat kuliah dan kompetisi (seperti Dashboard Tableau IKDS BPS yang memenangkan juara ke-3 tingkat nasional, sistem informasi akademik, dan aplikasi berbasis web).
- **Detail Kartu:** Deskripsi masalah, solusi dampak bisnis (*business impact*), *tech stack badges*, tautan repositori GitHub, serta *Live Preview*.

### 📍 Section 6: Contact & Footer
- **Form Kontak & Informasi Langsung:** Saluran komunikasi profesional (LinkedIn, GitHub, Email, WhatsApp).
- **Footer:** Hak cipta, identitas pengembang (*Aimar Trophy Sudrajat*), dan tombol navigasi *Back to Top*.

---

## 5. Tahapan Eksekusi & Roadmap Pengerjaan

| Tahap | Fokus Pengerjaan | Item Pekerjaan Utama |
| :--- | :--- | :--- |
| **Tahap 1** | Foundation & Design System | Setup struktur folder (`source-code`, `figma`, `laporan`, `google-stitch`), konfigurasi variabel `:root` warna *Tactile Blue / Midnight*, dan Navbar responsif. |
| **Tahap 2** | Hero & About Section | Pengerjaan komponen Home, status badge profesional, latar belakang akademik STMIK IKMI Cirebon, serta ringkasan profil korporat. |
| **Tahap 3** | Experience & Professional Timeline | Penyusunan riwayat kerja nyata (Prosegur, Indo Sultan, Tera Data) serta integrasi metrik akurasi tinggi. |
| **Tahap 4** | Technical Matrix & Interactive Skills | Implementasi bagian *Data Stack* dengan kartu interaktif bergaya *micro-tilt* (Analytics, BI, Data Science, Automation). |
| **Tahap 5** | Projects Showcase & Deployment | Menampilkan portofolio proyek data (Tableau, Web Apps), pengujian responsivitas, dan rilis final ke Vercel serta GitHub. |