# Website Profil & PPDB Pondok Pesantren Darul Ilmi Setia Usaha

Website resmi profil lembaga dan **Penerimaan Santri Baru (PPDB)** untuk **Yayasan Pondok Pesantren Darul Ilmi Setia Usaha** (Kabupaten Bengkayang, Kalimantan Barat). Dibangun sebagai *single-page website* modern dengan tema **Red Scarlet Gold** yang responsif, ringan, serta terintegrasi langsung dengan portal pendaftaran online resmi.

- **Website Kanonik:** `https://darulilmi.setiausaha.ponpes.id`
- **Portal Pendaftaran Online:** `https://pendaftaran.darulilmi.setiausaha.ponpes.id`

---

## Ringkasan Identitas Lembaga

| Informasi | Detail |
| :--- | :--- |
| **Nama Yayasan / Pesantren** | Yayasan Pondok Pesantren Darul Ilmi Setia Usaha |
| **Tanggal Berdiri** | 15 Rabi'ul Awal 1443 H / 22 Oktober 2021 |
| **Pengasuh / Pimpinan** | Ustaz Muhamad Ardi Ansha, M.Pd. *(Ketua LMY Kab. Bengkayang)* |
| **NSPP Kemenag RI** | `510261070012` |
| **Izin Operasional** | `033651` |
| **SK Kemenkumham RI** | `AHU-0025297.AH.01.04. Tahun 2021` |
| **Akte Notaris** | Endy Indra Permana, S.H., M.Kn. No. 83 Tahun 2021 |
| **Haluan & Sanad** | Ahlussunnah wal Jama'ah & Sanad Al-Qur'an Yanbu'ul Qur'an Kudus |
| **Alamat Lengkap** | Jln. UPT 1/B, Dusun Setia Usaha, Desa Sinar Tebudak, Kec. Tujuh Belas, Kab. Bengkayang, Prov. Kalimantan Barat, Kode Pos 79250 |

---

## Fitur Utama Website

1. **Tahun Ajaran Otomatis (*Real-Time*):**
   Fungsi JavaScript `getAcademicYear()` menyesuaikan tahun pelajaran pendaftaran secara otomatis berdasarkan tahun berjalan (`currentYear + 1` / `currentYear + 2`), misalnya tahun berjalan `2026` otomatis menampilkan **`2027/2028`** pada judul halaman, meta SEO/Open Graph, badge Hero, section PPDB, FAQ, dan Footer.
2. **Integrasi Portal Pendaftaran Online:**
   Seluruh tombol CTA utama (*Daftar Online* / *Daftar Online Sekarang*) di Navbar, Hero, Mobile Drawer, Section Pendaftaran, dan Mobile Sticky Bar mengarah langsung ke `https://pendaftaran.darulilmi.ponpes.id`.
3. **Galeri Dokumentasi UI Bento Grid + Lightbox:**
   Menampilkan 20 foto kegiatan, wisuda, pembelajaran, asrama, gedung, ruang kesehatan, dan lapangan olahraga dari folder `media/` dalam tata letak Bento Grid responsif dengan modal *Lightbox* (klik gambar untuk memperbesar).
4. **Transparansi Rincian Biaya & Syahriah:**
   Menyajikan rincian biaya santri mukim pondok, biaya sekolah formal SMP IT/MTs (Gratis 100% biaya daftar & jariyah gedung), informasi keringanan bagi santri yatim piatu & kurang mampu, pilihan paket makan bulanan (2x atau 3x sehari), skema angsuran, serta nomor rekening resmi BRI.
5. **Peta Lokasi & Konsultasi Panitia PPDB:**
   Tersedia *embed* Google Maps, tautan pin lokasi resmi, 3 kontak WhatsApp panitia PPDB (Admin Utama, Unit Putra, Unit Putri), tombol *Floating WhatsApp*, dan FAQ *accordion* interaktif.
6. **Responsif Desktop & Mobile:**
   Menggunakan **Tailwind CSS** (CDN) dengan navigasi *sticky*, *mobile hamburger drawer* dengan *focus trap*, serta *mobile sticky bottom bar* untuk akses cepat WhatsApp dan pendaftaran.

---

## Struktur Section (`index.html`)

| No | ID Section | Isi Utama |
| :---: | :--- | :--- |
| 1 | `#top` (Hero) | Latar Surau & Gedung Yayasan, badge PPDB dinamis, tagline, tombol Daftar Online & Rincian Biaya, highlight NSPP & kuota (`32 Putra & 32 Putri`) |
| 2 | Quick Info Bar | 4 keunggulan utama: Mahir Kitab Salaf, Target Tahfiz 30 Juz, Asrama Putra & Putri, Pendidikan Terpadu |
| 3 | `#profil` | Sejarah pendirian, foto keluarga besar & 3 logo resmi lembaga, legalitas, statistik (`2021`, `83` santri aktif, `8` program, `64` kuota), dan Sambutan Pengasuh |
| 4 | `#visi-misi` | Visi pesantren dan 5 butir Misi strategis |
| 5 | `#program` | 4 unit/lembaga pendidikan: SMP IT & MTs Darul Ilmi, Pondok Pesantren Putra & Putri, LMY Bengkayang, TPQ Al-Maghfiroh & Madrasah Diniyah |
| 6 | `#program-unggulan` | 8 program unggulan: Tahsin Thoriqoh Yanbu'a, Tahfizul Qur'an, Kitab Salaf, Nahwu Shorof, IT/Digital, Jurnalistik, MC/Pidato, Kajian Kitab |
| 7 | `#kehidupan-santri` | Jadwal harian santri (6 blok waktu `03.30–03.30 WIB`), kegiatan rutin mingguan/bulanan, dan daftar ekstrakurikuler |
| 8 | `#galeri` | UI Bento Grid 20 dokumentasi foto asli dengan keterangan dan Lightbox preview |
| 9 | `#fasilitas` | 8 sarana pendukung: Surau Al-Maghfiroh, Asrama Terpisah, Ruang Kelas, Perpustakaan, Lapangan Olahraga, Dapur Umum/Kantin/Koperasi, UKS, Wi-Fi Terkontrol & Keamanan 24 Jam |
| 10 | `#prestasi` | Tonggak pencapaian & sanad: Wisuda Yanbu'a Perdana (21 Juni 2023), Wisuda Ke-2 & Tahfiz 30 Juz Binnadhor, Pusat LMY Kab. Bengkayang |
| 11 | Testimoni | Testimoni asli wali santri (Ibu Satijah — Jagoi Ledo Lestari) |
| 12 | `#pendaftaran` & `#biaya` | Alur 4 tahap pendaftaran online, rincian biaya lengkap, Syahriah bulanan, metode pembayaran (BRI `4852 0103 0230 537` a.n. Muhammad Muhlasin), dan 6 syarat berkas (`#syarat-berkas`) |
| 13 | `#lokasi` | Peta Google Maps tersemat, alamat sekretariat PPDB, dan tautan pin Google Maps |
| 14 | `#faq` | 3 kontak WhatsApp Panitia PPDB, WA resmi pesantren, dan 6 pertanyaan umum (FAQ) |
| 15 | Footer | Identitas legalitas, navigasi cepat, kontak, dan tautan media sosial (Facebook, YouTube, TikTok) |

---

## Struktur Direktori

```text
Web PPDB Darul Ilmi Setia Usaha/
├── index.html                                           # Halaman utama website PPDB (single-page)
├── Form Pengisian Data Website PPDB Pesantren Darul Ilmi.md  # Dokumen sumber data & redaksi pesantren
├── README.md                                            # Dokumentasi proyek
└── media/                                               # Aset logo, foto kegiatan, fasilitas, & brosur
    ├── logo pondok white.jpeg                           # Logo resmi yayasan (navbar, footer, favicon)
    ├── logo SMP white.jpeg                              # Logo unit SMP IT Darul Ilmi
    ├── logo lajnah yanbua white.jpeg                    # Logo LMY Kab. Bengkayang
    ├── PENGASUH PESANTREN.jpeg                          # Foto Pengasuh Ustaz Muhamad Ardi Ansha, M.Pd.
    ├── KELUARGA BESAR.jpeg                              # Foto Dewan Pengasuh & Keluarga Besar
    ├── RINCIAN BIAYA.jpeg                               # Poster rincian biaya resmi (lightbox)
    └── *.webp                                           # 19 foto dokumentasi kegiatan, wisuda, asrama, gedung, & lapangan olahraga
```

---

## Cara Menjalankan Secara Lokal

Karena seluruh kode berada pada `index.html` tanpa proses *build* tambahan, Anda dapat langsung membuka file `index.html` di browser atau menjalankannya melalui server lokal agar seluruh aset dan *embed* berjalan optimal:

```bash
# Menggunakan Python
python -m http.server 8080

# Atau menggunakan Node.js
npx serve .
```

Lalu buka `http://localhost:8080` di browser.

---

## Kontak Resmi & Media Sosial

- **WhatsApp Resmi Pesantren:** `0858-2182-2683` (`https://wa.me/6285821822683`)
- **Panitia PPDB:**
  - Ustazah Nur Eviva, S.Si *(Kepala SMP IT / Admin Utama)*: `0812-5375-0253`
  - Ustaz Muhamad Muhlasin *(Unit Putra)*: `0858-2863-3381`
  - Ustaz Yusuf Anwar, S.Psi *(Unit Putri)*: `0815-4947-3054`
- **Email:** `ponpesdarulilmi2210@gmail.com`
- **Google Maps:** `https://maps.app.goo.gl/KWC2VZ6HKBtRzy8w8`
- **Media Sosial:** Facebook (`Ponpes Darul Ilmi Setia Usaha`) • YouTube (`@darulilmipaketb`) • TikTok (`@darul_ilmi_paket_b`)
