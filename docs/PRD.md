# DOKUMEN 1 — PRODUCT REQUIREMENT DOCUMENT
## KPI Builder untuk UMKM
### Landing Page / Company Profile + KPI Dashboard

---

## 1. Project Overview

### Nama Project
**KPI Builder untuk UMKM**

### Deskripsi Singkat
KPI Builder untuk UMKM adalah web app berbasis frontend-first yang membantu pemilik bisnis, manajer, dan tim UMKM memahami, membangun, dan memantau KPI secara terstruktur. Fokus utama dashboard adalah menampilkan hubungan sebab-akibat antar KPI, sehingga pengguna tidak hanya melihat angka, tetapi juga memahami bagaimana satu KPI memengaruhi KPI lain dalam sebuah **KPI Tree**.

### Tujuan Utama
Membangun tampilan web app yang terdiri dari:

1. **Landing Page / Company Profile**  
   Untuk menjelaskan value proposition, manfaat, fitur, cara kerja, use case, dan ajakan mencoba KPI Builder.

2. **KPI Dashboard**  
   Untuk menampilkan ringkasan KPI bisnis UMKM, status performa, KPI Tree, hubungan sebab-akibat, area bermasalah, dan prioritas tindakan.

### Fokus Teknologi Awal
Frontend terlebih dahulu menggunakan:

- HTML responsive
- Tailwind CSS Play CDN native
- Tanpa backend terlebih dahulu
- Data dashboard menggunakan dummy/static data
- Tidak ada integrasi API pada fase awal
- Tidak ada login fungsional pada fase awal
- Tidak ada database pada fase awal

---

## 2. Product Vision

### Visi Produk
Menjadi web app sederhana, modern, dan mudah dipahami yang membantu UMKM mengubah target bisnis menjadi sistem KPI yang jelas, terukur, dan saling terhubung.

### Prinsip Produk
Produk ini tidak hanya menjadi “dashboard angka”, tetapi menjadi **alat berpikir strategis** untuk UMKM.

Dashboard harus menjawab pertanyaan berikut:

1. Apa tujuan bisnis utama UMKM?
2. KPI apa yang paling penting untuk mencapai tujuan itu?
3. KPI mana yang menjadi penyebab naik/turunnya performa?
4. KPI mana yang terdampak oleh KPI lain?
5. Area mana yang perlu diperbaiki terlebih dahulu?
6. Apa tindakan prioritas yang disarankan?

---

## 3. Target User

### Primary User
**Owner UMKM / Founder / Pengelola Bisnis**

Karakteristik:
- Tidak selalu memiliki latar belakang manajemen formal.
- Membutuhkan visual yang mudah dipahami.
- Ingin tahu bisnisnya sehat atau tidak.
- Membutuhkan arahan konkret, bukan hanya grafik.
- Lebih nyaman dengan bahasa praktis dan ringkas.

### Secondary User
**Manager Operasional / Kepala Cabang / Supervisor**

Karakteristik:
- Bertanggung jawab pada target operasional.
- Perlu membaca KPI harian/mingguan/bulanan.
- Perlu tahu hubungan antara aktivitas tim dan hasil bisnis.

### Tertiary User
**Konsultan UMKM / Business Coach / HR Consultant**

Karakteristik:
- Menggunakan dashboard sebagai alat bantu diskusi dengan klien.
- Membutuhkan tampilan profesional untuk presentasi.
- Membutuhkan struktur KPI yang bisa dijelaskan secara logis.

---

## 4. Core Problem

Banyak UMKM memiliki target seperti “penjualan naik”, “profit meningkat”, atau “pelanggan bertambah”, tetapi tidak memiliki sistem KPI yang menjelaskan:

- KPI mana yang harus dipantau.
- Hubungan antara KPI satu dengan lainnya.
- Penyebab performa naik atau turun.
- Prioritas perbaikan.
- Keterkaitan antara aktivitas operasional dan hasil bisnis.

Akibatnya, UMKM sering:
- Mengejar omzet tetapi margin turun.
- Menambah promosi tetapi profit tidak naik.
- Fokus pada penjualan tetapi customer retention lemah.
- Mengukur terlalu banyak hal tetapi tidak tahu mana yang penting.
- Mengambil keputusan reaktif tanpa membaca akar masalah.

---

## 5. Product Value Proposition

### Main Value Proposition
**“Bantu UMKM membangun KPI yang bukan hanya terukur, tetapi juga saling terhubung secara sebab-akibat.”**

### Supporting Value
Produk ini membantu pengguna untuk:

1. Melihat performa bisnis dalam satu dashboard.
2. Memahami KPI utama dan KPI pendukung.
3. Melihat hubungan sebab-akibat antar KPI.
4. Menemukan akar masalah performa.
5. Menentukan prioritas tindakan.
6. Membangun KPI Tree yang mudah dijelaskan kepada tim.

---

## 6. Product Scope

### In Scope — Fase Frontend Awal

#### Landing Page / Company Profile
Halaman landing page mencakup:

1. Hero section
2. Problem statement
3. Value proposition
4. Fitur utama
5. Cara kerja
6. Use case UMKM
7. Preview dashboard
8. KPI Tree explanation
9. Pricing placeholder
10. FAQ
11. Call to action
12. Footer

#### KPI Dashboard
Dashboard mencakup:

1. Business performance summary
2. KPI health score
3. KPI cards
4. KPI Tree visualization
5. Cause-effect relationship panel
6. KPI impact map
7. Risk and alert section
8. Recommended action section
9. Department/function view
10. Dummy filter period
11. Dummy filter business unit
12. Static export button placeholder

---

### Out of Scope — Belum Dibangun di Fase Awal

Fitur berikut tidak dibangun dulu sebelum ada approval lanjutan:

1. Backend
2. Database
3. Login/authentication
4. Payment gateway
5. AI generation engine
6. Export PDF/Word fungsional
7. Real-time chart data
8. Multi-user collaboration
9. Role-based access
10. KPI approval workflow
11. Integrasi spreadsheet
12. Integrasi WhatsApp/email
13. Mobile app native

---

## 7. Information Architecture

### Struktur Halaman

#### Public Area
1. `/index.html`
   - Landing Page / Company Profile

#### App Area — Static Prototype
2. `/dashboard.html`
   - Main KPI Dashboard

3. `/kpi-tree.html`
   - Dedicated KPI Tree View

4. `/kpi-detail.html`
   - KPI Detail View

5. `/builder.html`
   - KPI Builder Form Prototype

6. `/settings.html`
   - Basic Settings Prototype

Catatan:
Pada fase awal, semua halaman dapat dibuat sebagai file HTML terpisah tanpa routing framework.

---

## 8. Landing Page Requirement

### 8.1 Hero Section

#### Tujuan
Menjelaskan produk secara cepat dan meyakinkan.

#### Konten Utama
Headline:
**“Bangun KPI UMKM yang Jelas, Terukur, dan Saling Terhubung.”**

Subheadline:
**KPI Builder membantu owner dan tim UMKM memahami hubungan sebab-akibat antar KPI, menemukan prioritas perbaikan, dan mengelola performa bisnis dalam satu dashboard modern.**

CTA utama:
**Coba Dashboard**

CTA sekunder:
**Lihat Cara Kerja**

Visual:
- Mockup dashboard futuristic.
- KPI Tree miniature.
- Dark navy gradient background.
- Glow effect biru/cyan.
- Floating metric cards.

---

### 8.2 Problem Section

#### Tujuan
Menunjukkan pain point UMKM.

#### Konten
Masalah utama:
- Target bisnis ada, tetapi KPI tidak jelas.
- Omzet naik, tetapi profit belum tentu naik.
- Aktivitas tim banyak, tetapi dampaknya tidak terlihat.
- KPI berdiri sendiri tanpa hubungan sebab-akibat.
- Owner sulit menentukan prioritas perbaikan.

Visual:
- Card grid berisi pain points.
- Icon warning, chart down, broken link, confusion.

---

### 8.3 Solution Section

#### Tujuan
Menjelaskan solusi produk.

#### Konten
KPI Builder membantu pengguna untuk:
- Menurunkan target bisnis menjadi KPI.
- Menghubungkan KPI utama dengan KPI pendukung.
- Membaca akar penyebab performa.
- Melihat KPI Tree secara visual.
- Menentukan action plan yang lebih tepat.

Visual:
- Before-after comparison.
- Sebelum: KPI terpisah.
- Sesudah: KPI saling terhubung.

---

### 8.4 Feature Section

#### Fitur Utama
1. KPI Dashboard
2. KPI Tree
3. Cause-Effect Mapping
4. Business Health Score
5. KPI Alert
6. Recommended Action
7. KPI Detail View
8. UMKM-Friendly Interface

---

### 8.5 How It Works Section

#### Alur
1. Masukkan tujuan bisnis.
2. Pilih area bisnis.
3. Bangun KPI utama.
4. Hubungkan KPI pendukung.
5. Pantau performa.
6. Ambil tindakan berdasarkan prioritas.

Visual:
- Horizontal stepper desktop.
- Vertical stepper mobile.

---

### 8.6 KPI Tree Explanation Section

#### Tujuan
Mengedukasi pengguna bahwa KPI tidak berdiri sendiri.

#### Contoh Tree
Objective:
**Meningkatkan Profit Bisnis**

KPI Level 1:
- Net Profit Margin

KPI Level 2:
- Revenue Growth
- Gross Margin
- Operating Cost Ratio

KPI Level 3:
- Average Transaction Value
- Repeat Purchase Rate
- Conversion Rate
- COGS Ratio
- Marketing Cost Ratio

Pesan utama:
**KPI Tree membantu owner melihat KPI mana yang menjadi driver dan KPI mana yang menjadi hasil.**

---

### 8.7 Use Case Section

#### Use Case 1 — Retail UMKM
Masalah:
Omzet naik, tetapi profit turun.

KPI Tree membantu melihat:
- Revenue naik.
- COGS naik lebih cepat.
- Diskon terlalu besar.
- Margin menurun.

#### Use Case 2 — F&B
Masalah:
Banyak pelanggan baru, tetapi repeat order rendah.

KPI Tree membantu melihat:
- Customer acquisition tinggi.
- Retention rendah.
- Complaint meningkat.
- Service speed rendah.

#### Use Case 3 — Jasa
Masalah:
Project banyak, tetapi cashflow ketat.

KPI Tree membantu melihat:
- Sales tinggi.
- Collection period lambat.
- Project cost tidak terkendali.
- Cash conversion cycle buruk.

---

### 8.8 Pricing Placeholder

Fase frontend awal hanya menampilkan placeholder pricing.

Paket contoh:
1. Starter
2. Growth
3. Consultant

Tidak perlu payment integration terlebih dahulu.

---

## 9. Dashboard Requirement

### 9.1 Dashboard Main Objective

Dashboard harus membantu user membaca:

1. Kondisi performa bisnis.
2. KPI yang sehat dan bermasalah.
3. Hubungan sebab-akibat antar KPI.
4. Akar masalah performa.
5. Rekomendasi tindakan prioritas.

---

### 9.2 Dashboard Layout

#### Top Navigation
Elemen:
- Logo KPI Builder
- Menu: Dashboard, KPI Tree, Builder, Reports, Settings
- CTA: Upgrade / Export
- User avatar placeholder

#### Dashboard Header
Elemen:
- Page title: “KPI Dashboard”
- Business name: “UMKM Demo”
- Period filter: Monthly / Quarterly / Yearly
- Business area filter: All / Sales / Finance / Operation / Customer
- Last updated dummy timestamp

#### Executive KPI Summary
Elemen:
- Business Health Score
- Revenue Achievement
- Profit Margin
- Customer Retention
- Cost Efficiency

#### KPI Cards
Setiap card memiliki:
- KPI name
- Current value
- Target value
- Achievement percentage
- Trend indicator
- Status badge
- Driver/Outcome label
- Impact level

Status:
- Healthy
- Watch
- Critical

---

### 9.3 KPI Tree Dashboard

#### Tujuan
Menampilkan struktur hubungan KPI dari objective tertinggi sampai KPI operasional.

#### Struktur Visual
Level 0:
- Strategic Objective

Level 1:
- Main Outcome KPI

Level 2:
- Business Driver KPI

Level 3:
- Operational Driver KPI

Level 4:
- Action/Initiative Indicator

#### Contoh Struktur

Strategic Objective:
**Meningkatkan Profitabilitas Bisnis**

Outcome KPI:
- Net Profit Margin

Driver KPI:
- Revenue Growth
- Gross Margin
- Operating Cost Ratio

Operational KPI:
- Conversion Rate
- Average Transaction Value
- Repeat Purchase Rate
- COGS Ratio
- Inventory Waste
- Marketing Cost per Customer

Action Indicator:
- Promo Effectiveness
- Stock Accuracy
- Sales Follow-Up Rate
- Service Response Time

---

### 9.4 Cause-Effect Relationship Panel

#### Tujuan
Menjelaskan hubungan antar KPI dalam bahasa sederhana.

#### Contoh Tampilan
Jika:
- Repeat Purchase Rate turun
- Customer Complaint naik
- Service Response Time memburuk

Maka dampaknya:
- Revenue Growth tertekan
- Customer Retention turun
- Profitability ikut melemah

#### Komponen
1. Selected KPI
2. Upstream Drivers
3. Downstream Impact
4. Risk Explanation
5. Suggested Action

---

### 9.5 KPI Detail View

Setiap KPI harus memiliki detail:

1. KPI Name
2. KPI Category
3. KPI Type
   - Outcome KPI
   - Driver KPI
   - Activity KPI
4. Formula
5. Target
6. Actual
7. Achievement
8. Owner
9. Review Frequency
10. Linked KPI
11. Upstream Cause
12. Downstream Impact
13. Risk if Not Improved
14. Recommended Action

---

### 9.6 KPI Builder Form Prototype

Tujuan:
Memberikan simulasi bagaimana user membangun KPI.

Field:
1. Business goal
2. Business type
3. Function area
4. Role / department
5. KPI category
6. KPI name
7. Formula
8. Target
9. Review period
10. Linked parent KPI
11. Linked child KPI
12. KPI type
13. Priority level

Output:
- KPI card preview
- Position in KPI Tree
- Cause-effect note

---

## 10. Data Model SOT — Frontend Dummy Data

### 10.1 KPI Object

Setiap KPI dalam dummy data harus mengikuti struktur berikut secara konseptual:

- id
- name
- category
- type
- parentId
- childIds
- value
- target
- unit
- achievement
- status
- trend
- owner
- reviewFrequency
- formula
- impactLevel
- upstreamDrivers
- downstreamImpacts
- recommendedActions

---

### 10.2 KPI Type

Jenis KPI:
1. Strategic Objective
2. Outcome KPI
3. Driver KPI
4. Operational KPI
5. Activity Indicator

---

### 10.3 KPI Status

Status:
1. Healthy
2. Watch
3. Critical

Logic visual:
- Healthy: performa aman.
- Watch: perlu perhatian.
- Critical: perlu tindakan segera.

---

## 11. Key User Journey

### Journey 1 — Visitor Membuka Landing Page
1. User melihat hero section.
2. User memahami problem KPI UMKM.
3. User melihat contoh dashboard.
4. User memahami KPI Tree.
5. User klik “Coba Dashboard”.
6. User diarahkan ke dashboard static prototype.

### Journey 2 — User Membaca Dashboard
1. User melihat Business Health Score.
2. User membaca KPI utama.
3. User melihat KPI bermasalah.
4. User membuka KPI Tree.
5. User memahami penyebab masalah.
6. User melihat recommended action.

### Journey 3 — User Membuat KPI Baru
1. User membuka KPI Builder.
2. User mengisi business goal.
3. User memilih area bisnis.
4. User menambahkan KPI.
5. User menghubungkan KPI ke parent KPI.
6. User melihat preview KPI Tree.

---

## 12. Success Criteria

### Frontend Success Criteria
Prototype dianggap berhasil jika:

1. Landing page terlihat modern, profesional, dan sesuai branding.
2. Dashboard mudah dipahami oleh non-teknikal user.
3. KPI Tree terlihat jelas secara visual.
4. Hubungan sebab-akibat KPI dapat dipahami tanpa penjelasan panjang.
5. Layout responsif di desktop, tablet, dan mobile.
6. Seluruh halaman dapat berjalan sebagai static HTML.
7. Komponen UI konsisten.
8. Tidak ada eksekusi backend sebelum approval.

---

## 13. Approval Gate

### Status Saat Ini
**Status: Pending Approval**

### Yang Perlu Disetujui Sebelum Coding
1. Struktur halaman.
2. Style visual.
3. Isi section landing page.
4. Struktur dashboard.
5. Struktur KPI Tree.
6. Dummy data KPI.
7. Urutan fase implementasi.

### Catatan
Tidak ada coding yang dilakukan sebelum approval eksplisit dari owner project.
