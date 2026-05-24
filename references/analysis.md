# Analisis Pekeliling Pendigitalan Perkhidmatan Awam Bil. 1/2025

> **Sumber dokumen:**
> - `pdf/898b44118328c280b675e27be3abc657.pdf` — Surat iringan KSN (2 ms)
> - `pdf/eb4071a29089485be3ab93272b7996d5.pdf` — Pekeliling penuh + Lampiran A (68 ms)
>
> **Dianalisis:** 2026-05-24

---

## 1. Identiti Dokumen

| Perkara | Butiran |
|---|---|
| **Tajuk** | Pekeliling Pendigitalan Perkhidmatan Awam Bilangan 1 Tahun 2025 – Pengurusan Portal/Laman Web Agensi Sektor Awam |
| **Pengeluar** | Jabatan Digital Negara (JDN), Kementerian Digital |
| **Penandatangan surat iringan** | Tan Sri Shamsul Azri Bin Abu Bakar (Ketua Setiausaha Negara) |
| **Rujukan** | JDN.100-1/3/2 (2) — pekeliling; JDN.100-1/3/1 (19) — surat iringan |
| **Tarikh** | Ogos 2025 |
| **Kuat kuasa** | Serta-merta |
| **Pertanyaan** | Pengarah, Bahagian Kerajaan Digital, JDN, Cyberjaya — `bkdjdn@jdn.gov.my` · https://www.jdn.gov.my |

## 2. Pemakaian (Skop Agensi)

Terpakai kepada semua agensi:
- **PAP** — Perkhidmatan Awam Persekutuan
- **PAN** — Perkhidmatan Awam Negeri
- **BBP** — Badan Berkanun Persekutuan
- **BBN** — Badan Berkanun Negeri
- **PBT** — Pihak Berkuasa Tempatan

Pemakaian boleh diluaskan kepada portal/laman web *perkhidmatan* agensi (bukan hanya laman rasmi).

## 3. Dokumen Yang Dibatalkan (6)

1. SAKP Bil. 2/2009 — Garis Panduan Pelaksanaan Blog Agensi Sektor Awam
2. SAKP Bil. 3/2009 — Panduan Berita Online di Laman Web Agensi-Agensi Kerajaan
3. SAKP Bil. 4/2009 — Garis Panduan Pembangunan Kandungan Sektor Awam
4. **PKPA Bil. 2/2015 — Pengurusan Laman Web Agensi Sektor Awam** (dokumen utama lama)
5. SAKP Bil. 2/2015 — Garis Panduan Rasionalisasi Laman Web Sektor Awam
6. SPKPA Bil. 1/2019 — Penyeragaman Lokasi & Reka Bentuk Pautan Borang Aduan

## 4. Struktur Tadbir Urus

### 4.1 Peringkat Induk (Kementerian / PSUK Negeri)

```
┌──────────────────────────────────────────────────┐
│  Jawatankuasa Induk Pengurusan Portal/Laman Web │
│           Kementerian/Negeri (CDO)              │
└────────────────┬─────────────────────────────────┘
        ┌────────┴────────┐
        ▼                 ▼
┌──────────────┐  ┌──────────────┐
│ Pasukan      │  │ Pasukan      │
│ Kandungan    │  │ Teknikal     │
│ (SU Kom.     │  │ (SU Pengrsn  │
│  Korporat)   │  │  Maklumat)   │
└──────────────┘  └──────────────┘
```

### 4.2 Peringkat Jabatan
Struktur sama (3 komponen), pengerusi JK Pengurusan = CDO Jabatan.

**Cadangan kekerapan mesyuarat:** 2× setahun untuk setiap pasukan.

## 5. Empat Tiang Pembangunan Portal/Laman Web

### 5.1 Reka Bentuk (Bab 3.2)

- ✅ Pernyataan "Portal/Laman Web Rasmi" di halaman utama
- ✅ Jata Persekutuan / Jata Negeri / logo rasmi (rujuk SPA 1/2022)
- ✅ Domain `gov.my` mandatori
- ✅ Maksimum **3 warna**; latar **putih** disaran
- ✅ Saiz ikon ≤ **1KB**, fon seragam
- ✅ Pop-up ikut keperluan sahaja
- ✅ Carian di semua halaman
- ✅ **4 Pautan Utama** di **penjuru kanan atas** (Lampiran A2):
  1. Soalan Lazim
  2. Hubungi Kami
  3. Aduan dan Maklum Balas
  4. Peta Laman
- ✅ Pautan "Hubungi Kami" — alamat & telefon rasmi sahaja
- 📎 Rujuk: https://standard.digital.gov.my

### 5.2 Kefungsian (Bab 3.3)

| Ciri | Status |
|---|---|
| Dwibahasa (BM + BI) | Mandatori |
| Soalan lazim | Mandatori |
| Chatbot (AI digalakkan) | Sangat digalakkan |
| Emerging tech (AI, Blockchain) | Digalakkan |
| Support link (help, SOP, manual, video) | Ya |
| Maklum balas + auto-jana no. rujukan | Ya |
| Kaji selidik kepuasan pengguna | Ya |
| Hot topic / tag cloud | Ya |
| Filter mengikut kumpulan sasaran | Ya |
| Hebahan/pengumuman ("Tiada Makluman Terkini" jika kosong) | Ya |
| Notifikasi e-mel/SMS/RSS | Ya |
| Carian lanjutan (predictive) | Ya |
| Personalisasi pintar | Ya |
| **W3C / WCAG accessibility (OKU)** | Mandatori |
| Pengarkiban elektronik (>1 tahun) | Ya |
| Pautan luar — **MyGovernment + Data Terbuka mandatori** | Ya |
| Peta Laman / indeks | Ya |
| Versi mobile + QR Code | Ya |
| Dasar agensi, piagam pelanggan, penafian, privasi, hak cipta | Ya |
| **Integrasi Identiti Digital Nasional (IDN)** | Perlu diambil kira |

### 5.3 Kandungan (Bab 3.4)

**Mandatori paparkan:**
- Maklumat Korporat (Visi, Misi, Fungsi, Carta Organisasi, Perutusan Ketua Jabatan)
- Mengenai Kami
- Hubungi Kami — **alamat e-mel statik** (elak spam), direktori fleksibel (boleh guna e-mel kumpulan/pusat panggilan)
- Maklumat CDO Agensi (profil, berita, aktiviti)
- Maklumat terkini dengan **auto-luput**
- Dokumen/klip video boleh muat turun
- Perkhidmatan teras + perkhidmatan dalam talian (e-Permohonan, e-Pembayaran, e-Aduan)
- Saluran penyampaian (ikon: telefon=SMS, tetikus=online, dll.)
- Perkhidmatan **end-to-end** (cth. lesen: permohonan → kelulusan → bayaran → cetakan)
- **e-Penyertaan 3 tahap:** e-Information → e-Consultation → e-Decision Making (kekal di portal **≥6 bulan**)
- Data terbuka (hubungi `dataterbuka@jdn.gov.my`)
- Media sosial — ditadbir oleh pentadbir bertanggungjawab

**🚫 DILARANG (3.4.2):**
- Iklan perkhidmatan pihak luar
- Isu sensitif (agama, politik, perkauman)
- Perkara tiada kaitan dengan perkhidmatan agensi
- Kenyataan jejaskan imej kerajaan

**Pengecualian (3.4.3):** Iklan pihak luar dibenarkan **jika** ada MoU/kontrak dan beri nilai tambah kepada perkhidmatan teras.

### 5.4 Keselamatan (Bab 4.6)

| Aspek | Keperluan |
|---|---|
| Klasifikasi | Hanya maklumat **rasmi + data terbuka**; rahsia rasmi rujuk **CGSO** dulu |
| Data-in-motion | **Sijil digital GPKI** / CA tempatan |
| Infrastruktur | Firewall, IPS, **WAF** |
| Anti-malware | Real-time scanning, ransomware protection |
| Patching | OS, DB, CMS, plug-in mesti terkini |
| Backup + DRP | Bangun, laksana, uji secara berkala |
| Pengujian keselamatan | Berkala (penetration test) |
| Fail log + audit trail | Diaktifkan + disimpan untuk forensik |
| Insiden | Lapor ke **CSIRT** / **NC4** (NACSA) |

## 6. Pemantauan, Pematuhan & KPI

### KPI Mandatori (Bab 4.4)
**Penyampaian:**
- % perkhidmatan online dibangunkan/bulan
- % transaksi online/bulan
- % aduan diambil tindakan dalam tempoh piagam pelanggan
- % maklumat terkini dikemas kini sebelum tarikh tamat

**Capaian:**
- **Uptime %** tersedia diakses
- **Kepantasan paparan < 5 saat** setiap klik
- **Kedalaman klik ≤ 3** untuk capai maklumat

JDN memantau berkala melalui sistem elektronik agensi pusat.

## 7. Rasionalisasi Portal/Laman Web (Bab 5)

Setiap agensi mesti klasifikasi portal/laman web/blog kepada **4 kategori**:

| Kategori | Bila? |
|---|---|
| **Dikekalkan** | Hanya **1 portal rasmi** sahaja per agensi |
| **Ditutup** | Duplikat, tidak diperlukan, atau tidak diselenggara **>6 bulan**. Domain pun ditutup. |
| **Dikonsolidasi** | Portal cawangan/bahagian/unit/seksyen → gabung sebagai subdomain atau subdirektori |
| **Dikecualikan** | Portal khusus berimpak besar (cth. `data.gov.my`, `myidentity.gov.my`) — perlu **kelulusan JK Induk** + maklum ke **JDN** |

**Aliran:** Agensi Pelaksana → kelulusan JK Pengurusan Jabatan → kelulusan JK Induk Kementerian/Negeri → laksana → lapor balik (Lampiran A5).

## 8. Penyelarasan dengan Portal MyGovernment (Bab 6)

- Portal MyGovernment (https://www.malaysia.gov.my) = gerbang tunggal kerajaan
- Tanggungjawab agensi:
  - Kemas kini perkhidmatan & maklumat untuk dipautkan
  - Pastikan URL **aktif** (elak broken links)
  - Maklumkan sebarang perubahan URL
  - Promosi inisiatif MyGovernment
- Matlamat antarabangsa: tingkatkan **OSI (Online Service Index)** PBB

## 9. Akronim Utama

| Akronim | Maksud |
|---|---|
| **JDN** | Jabatan Digital Negara |
| **CDO** | Chief Digital Officer / Ketua Pegawai Digital |
| **CGSO** | Chief Government Security Office |
| **CMS** | Content Management System |
| **CSIRT** | Cyber Security Incident Response Team |
| **DRP** | Disaster Recovery Plan |
| **GPKI** | Government Public Key Infrastructure |
| **IPS / WAF** | Intrusion Prevention System / Web Application Firewall |
| **NACSA / NC4** | National Cyber Security Agency / National Cyber Coordination & Command Centre |
| **OSI** | Online Service Index (PBB) |
| **MCSL** | Malaysian Civil Service Link |
| **PPA** | Portal Perkhidmatan Awam |
| **PSUK** | Pejabat Setiausaha Kerajaan |
| **TOT** | Transfer of Technology |

## 10. Lampiran (A1–A7)

| Lampiran | Kandungan |
|---|---|
| **A** | Pekeliling penuh (Bab 1–8) |
| **A1** | Templat penggunaan Jata/Logo rasmi mengikut jenis agensi |
| **A2** | Reka bentuk + lokasi 4 pautan utama (BM + BI) |
| **A3** | Contoh reka bentuk pautan luar (ikon / nama) |
| **A4** | Borang inventori rasionalisasi (contoh data MAMPU→JDN) |
| **A5** | Carta alir 3-lajur (Pelaksana / Induk / JDN) |
| **A6** | Senarai semak rasionalisasi — Agensi Induk |
| **A7** | Senarai semak rasionalisasi — Agensi Pelaksana |

---

## 11. Implikasi Praktikal untuk Pembinaan Laman

Jika membina laman web sektor awam yang patuh pekeliling ini, **minimum keperluan teknikal**:

1. **Domain & SSL:** `*.gov.my` + sijil GPKI
2. **Header/Branding:** Jata Persekutuan/Negeri + teks "Portal/Laman Web Rasmi" + nama Kementerian/Agensi
3. **Top-right quick links:** Soalan Lazim · Hubungi Kami · Aduan · Peta Laman (ikon seragam, BM+BI)
4. **i18n:** BM (default) + EN
5. **Aksesibiliti:** WCAG 2.x AA — text resize, contrast toggle, alt text, audio/visual alternatives
6. **Carian:** Site-wide search di setiap halaman + advanced/predictive
7. **Mobile-first + QR code** ke versi mudah alih
8. **Footer mandatori:** Dasar privasi · Penafian · Hak cipta · Piagam pelanggan · Peta laman
9. **Pautan luar mandatori:** MyGovernment (`malaysia.gov.my`) + Data Terbuka (`data.gov.my`)
10. **CMS:** Auto-luput untuk pengumuman, arkib elektronik >1 tahun, ruangan "Tiada Makluman Terkini"
11. **Borang feedback:** Auto-jana no. rujukan
12. **Kaji selidik:** Pop-up notifikasi selepas transaksi
13. **Security stack:** WAF + IPS + log audit + backup + DRP
14. **Sasaran prestasi:** Uptime tinggi, **<5s page load**, **≤3 click depth**
15. **Integrasi:** IDN (untuk authentication), Portal MyGovernment (untuk service exposure)
