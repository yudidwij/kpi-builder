# DOKUMEN 3 — IMPLEMENTATION PLAN
## KPI Builder untuk UMKM
### Frontend-First Execution Plan
### HTML Responsive + Tailwind CSS Play CDN Native

---

## 1. Implementation Philosophy

Project ini menggunakan pendekatan **SOT-driven frontend development**.

Artinya, sebelum coding dilakukan, semua keputusan utama harus tertulis dalam dokumen sumber kebenaran:

1. PRD
2. UI Guidelines
3. Implementation Plan

Eksekusi frontend hanya boleh mengikuti dokumen ini, bukan improvisasi bebas.

---

## 2. Development Constraint

### Teknologi yang Diizinkan pada Fase Awal
- HTML native
- Tailwind CSS Play CDN
- JavaScript ringan jika diperlukan untuk interaksi dummy
- Static data
- Responsive layout
- File-based pages

### Teknologi yang Belum Diizinkan
- React
- Next.js
- Vue
- Backend
- Database
- Auth
- Payment gateway
- API integration
- Charting library kompleks
- Build tools
- NPM package
- Server deployment otomatis

### Alasan Constraint
Fase awal bertujuan untuk:
1. Memvalidasi UI dan product flow.
2. Membuat prototype cepat.
3. Menghindari kompleksitas backend.
4. Memastikan stakeholder menyetujui struktur produk.
5. Menyiapkan dasar sebelum masuk aplikasi dinamis.

---

## 3. Recommended File Structure

Struktur file frontend awal:

```text
kpi-builder-umkm/
├── index.html
├── dashboard.html
├── kpi-tree.html
├── kpi-detail.html
├── builder.html
├── settings.html
├── assets/
│   ├── images/
│   ├── icons/
│   └── mockups/
├── docs/
│   ├── PRD.md
│   ├── UI-Guidelines.md
│   └── Implementation-Plan.md
└── README.md
```

Catatan:
- Belum perlu folder `src`.
- Belum perlu package manager.
- Belum perlu build config.
- Semua halaman dapat dibuka langsung di browser.

---

## 4. Page Implementation Scope

### Page 1 — Landing Page / Company Profile

File:
`index.html`

Objective:
Menjelaskan produk dan mengarahkan user ke dashboard demo.

Section:
1. Navbar
2. Hero
3. Problem
4. Solution
5. Feature
6. KPI Tree explanation
7. Dashboard preview
8. Use case
9. Pricing placeholder
10. FAQ
11. CTA
12. Footer

Status:
**Pending Approval**

---

### Page 2 — Main KPI Dashboard

File:
`dashboard.html`

Objective:
Menampilkan ringkasan performa bisnis dan KPI utama.

Section:
1. Topbar
2. Dashboard header
3. Filter dummy
4. Business Health Score
5. KPI summary cards
6. KPI Tree preview
7. Cause-effect insight panel
8. Risk alert
9. Recommended action
10. KPI table summary

Status:
**Pending Approval**

---

### Page 3 — KPI Tree View

File:
`kpi-tree.html`

Objective:
Menampilkan hubungan sebab-akibat KPI secara lebih lengkap.

Section:
1. Header
2. Objective node
3. Outcome KPI node
4. Driver KPI nodes
5. Operational KPI nodes
6. Action indicator nodes
7. Legend
8. Selected KPI side panel

Status:
**Pending Approval**

---

### Page 4 — KPI Detail View

File:
`kpi-detail.html`

Objective:
Menampilkan detail satu KPI dan hubungannya dengan KPI lain.

Section:
1. KPI title
2. Status summary
3. Formula
4. Actual vs target
5. Owner
6. Review frequency
7. Upstream drivers
8. Downstream impacts
9. Risk explanation
10. Recommended action

Status:
**Pending Approval**

---

### Page 5 — KPI Builder Prototype

File:
`builder.html`

Objective:
Mensimulasikan proses pembuatan KPI.

Section:
1. Business goal input
2. Business type selector
3. Function area selector
4. KPI type selector
5. KPI name input
6. Formula input
7. Target input
8. Parent KPI selector
9. Preview KPI card
10. Preview KPI Tree position

Status:
**Pending Approval**

---

### Page 6 — Settings Prototype

File:
`settings.html`

Objective:
Menampilkan placeholder pengaturan bisnis.

Section:
1. Business profile
2. KPI category setting
3. Review period setting
4. Team/function placeholder
5. Export setting placeholder

Status:
**Pending Approval**

---

## 5. Component Implementation Plan

### 5.1 Global Components

#### Navbar
Digunakan di landing page.

Elemen:
- Logo
- Menu
- CTA
- Mobile menu placeholder

Status:
Pending Approval

#### App Topbar
Digunakan di halaman dashboard.

Elemen:
- Logo
- Navigation menu
- Export button
- User avatar placeholder

Status:
Pending Approval

#### Button
Tipe:
- Primary CTA
- Secondary CTA
- Ghost button
- Filter button

Status:
Pending Approval

#### Card
Tipe:
- Feature card
- Metric card
- Insight card
- KPI node card
- Pricing card

Status:
Pending Approval

---

### 5.2 KPI Components

#### KPI Metric Card
Elemen:
- KPI name
- Current value
- Target
- Achievement percentage
- Status
- Trend
- Type badge

Status:
Pending Approval

#### KPI Tree Node
Elemen:
- KPI name
- KPI type
- Achievement
- Status dot
- Impact level

Status:
Pending Approval

#### Cause-Effect Panel
Elemen:
- Selected KPI
- Cause KPI
- Impact KPI
- Explanation
- Recommended action

Status:
Pending Approval

#### KPI Status Badge
Status:
- Healthy
- Watch
- Critical

Status:
Pending Approval

---

## 6. Dummy Data Plan

Dummy data digunakan untuk membuat prototype terasa nyata.

### 6.1 Business Profile Dummy
Contoh:
- Business name: “UMKM Demo”
- Industry: “Retail & F&B”
- Period: “Juni 2026”
- Main objective: “Meningkatkan Profitabilitas Bisnis”

### 6.2 KPI Dummy Data

KPI utama:
1. Net Profit Margin
2. Revenue Growth
3. Gross Margin
4. Operating Cost Ratio
5. Repeat Purchase Rate
6. Conversion Rate
7. Average Transaction Value
8. COGS Ratio
9. Customer Complaint Rate
10. Service Response Time

### 6.3 KPI Tree Dummy Structure

Strategic Objective:
**Meningkatkan Profitabilitas Bisnis**

Level 1:
- Net Profit Margin

Level 2:
- Revenue Growth
- Gross Margin
- Operating Cost Ratio

Level 3:
- Conversion Rate
- Average Transaction Value
- Repeat Purchase Rate
- COGS Ratio
- Marketing Cost Ratio
- Inventory Waste

Level 4:
- Sales Follow-Up Rate
- Promo Effectiveness
- Stock Accuracy
- Supplier Cost Control
- Service Response Time

---

## 7. Phase-Based Execution Plan

### Phase 0 — SOT Finalization

Objective:
Mengunci dokumen PRD, UI Guidelines, dan Implementation Plan.

Deliverable:
- Final PRD
- Final UI Guidelines
- Final Implementation Plan

Activity:
1. Review dokumen.
2. Revisi jika diperlukan.
3. Approval dari owner project.
4. Lock scope frontend.

Status:
**Pending Approval**

Exit Criteria:
- Owner menyetujui struktur produk.
- Owner menyetujui style visual.
- Owner menyetujui halaman yang akan dibuat.
- Owner menyetujui urutan fase coding.

---

### Phase 1 — Landing Page Static HTML

Objective:
Membangun landing page/company profile.

Deliverable:
- `index.html`

Activity:
1. Build navbar.
2. Build hero section.
3. Build problem section.
4. Build solution section.
5. Build feature section.
6. Build KPI Tree explanation.
7. Build dashboard preview.
8. Build use case section.
9. Build pricing placeholder.
10. Build FAQ.
11. Build CTA and footer.
12. Responsive check.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Landing page responsive.
- CTA menuju dashboard demo.
- Visual sesuai UI Guidelines.
- Tidak ada backend/API.

---

### Phase 2 — Dashboard Static HTML

Objective:
Membangun main KPI dashboard.

Deliverable:
- `dashboard.html`

Activity:
1. Build app topbar.
2. Build dashboard header.
3. Build filter dummy.
4. Build KPI summary cards.
5. Build Business Health Score panel.
6. Build KPI Tree preview.
7. Build cause-effect panel.
8. Build risk alert.
9. Build recommended action.
10. Build KPI table.
11. Responsive check.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Dashboard terbaca jelas.
- KPI health score terlihat.
- KPI Tree preview muncul.
- Cause-effect explanation terlihat.
- Semua data masih dummy/static.

---

### Phase 3 — KPI Tree Page

Objective:
Membangun halaman khusus KPI Tree.

Deliverable:
- `kpi-tree.html`

Activity:
1. Build header.
2. Build tree container.
3. Build objective node.
4. Build outcome node.
5. Build driver nodes.
6. Build operational nodes.
7. Build action indicator nodes.
8. Build connection lines.
9. Build legend.
10. Build selected KPI panel.
11. Responsive behavior for mobile.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Hubungan KPI terlihat jelas.
- Level KPI terbaca.
- Status KPI terlihat.
- Arah sebab-akibat mudah dipahami.
- Mobile tetap usable.

---

### Phase 4 — KPI Detail Page

Objective:
Membangun halaman detail KPI.

Deliverable:
- `kpi-detail.html`

Activity:
1. Build KPI header.
2. Build metric summary.
3. Build formula section.
4. Build target vs actual.
5. Build owner/review section.
6. Build upstream driver panel.
7. Build downstream impact panel.
8. Build risk section.
9. Build recommended action section.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Detail KPI lengkap.
- Formula terlihat.
- Driver dan impact jelas.
- Recommended action mudah dipahami.

---

### Phase 5 — KPI Builder Prototype

Objective:
Membangun form prototype untuk membuat KPI.

Deliverable:
- `builder.html`

Activity:
1. Build form layout.
2. Build business goal field.
3. Build business type selector.
4. Build function area selector.
5. Build KPI type selector.
6. Build formula field.
7. Build target field.
8. Build parent KPI selector.
9. Build preview card.
10. Build tree position preview.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- User dapat memahami alur membuat KPI.
- Preview KPI card terlihat.
- Parent-child KPI concept terlihat.
- Tidak perlu form submission fungsional.

---

### Phase 6 — Settings Prototype

Objective:
Membangun halaman pengaturan dummy.

Deliverable:
- `settings.html`

Activity:
1. Build business profile section.
2. Build KPI category section.
3. Build review period section.
4. Build team/function placeholder.
5. Build export setting placeholder.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Settings page terlihat sebagai bagian dari aplikasi.
- Tidak ada fungsi backend.
- Layout konsisten.

---

### Phase 7 — QA, Responsiveness, and UI Polish

Objective:
Memastikan semua halaman konsisten, responsif, dan siap demo.

Activity:
1. Review desktop layout.
2. Review tablet layout.
3. Review mobile layout.
4. Check CTA links.
5. Check visual consistency.
6. Check spacing.
7. Check text readability.
8. Check KPI Tree clarity.
9. Check dashboard hierarchy.
10. Clean unused/duplicated patterns.

Status:
**Not Started — Waiting Approval**

Exit Criteria:
- Semua halaman dapat dibuka.
- Semua link antar halaman berjalan.
- Tidak ada layout rusak.
- UI konsisten.
- Prototype siap dipresentasikan.

---

## 8. Development Rules for Codex Execution

Ketika nanti masuk coding, agent/Codex harus mengikuti aturan berikut:

1. Jangan menambahkan fitur di luar scope.
2. Jangan menggunakan framework selain HTML + Tailwind Play CDN.
3. Jangan membuat backend.
4. Jangan membuat database.
5. Jangan menambahkan dependency NPM.
6. Jangan mengubah brand direction tanpa approval.
7. Jangan membuat halaman baru di luar file structure.
8. Jangan menghilangkan KPI Tree.
9. Jangan membuat dashboard hanya sebagai chart biasa.
10. Harus menonjolkan hubungan sebab-akibat KPI.
11. Harus menjaga responsive design.
12. Harus menggunakan dummy data yang konsisten.
13. Harus menjaga copywriting tetap sederhana untuk UMKM.
14. Harus update status fase setelah setiap fase selesai.
15. Harus berhenti setelah fase selesai untuk menunggu approval fase berikutnya.

---

## 9. Phase Status Tracker

| Phase | Nama Fase | Deliverable | Status |
|---|---|---|---|
| Phase 0 | SOT Finalization | PRD, UI Guidelines, Implementation Plan | Pending Approval |
| Phase 1 | Landing Page | index.html | Not Started |
| Phase 2 | Dashboard | dashboard.html | Not Started |
| Phase 3 | KPI Tree Page | kpi-tree.html | Not Started |
| Phase 4 | KPI Detail Page | kpi-detail.html | Not Started |
| Phase 5 | KPI Builder Prototype | builder.html | Not Started |
| Phase 6 | Settings Prototype | settings.html | Not Started |
| Phase 7 | QA & Polish | Final static prototype | Not Started |

---

## 10. Approval Workflow

### Setelah Phase 0
Owner menyetujui:
- Scope
- Style
- Struktur halaman
- KPI Tree logic
- Dummy data
- Urutan implementasi

### Setelah Phase 1
Owner review landing page.

Jika approved:
Lanjut Phase 2.

Jika revisi:
Perbaiki Phase 1 terlebih dahulu.

### Setelah Phase 2
Owner review dashboard.

Jika approved:
Lanjut Phase 3.

Jika revisi:
Perbaiki Phase 2 terlebih dahulu.

### Setelah Phase 3
Owner review KPI Tree.

Jika approved:
Lanjut Phase 4.

Jika revisi:
Perbaiki Phase 3 terlebih dahulu.

### Setelah Phase 4
Owner review KPI Detail.

Jika approved:
Lanjut Phase 5.

Jika revisi:
Perbaiki Phase 4 terlebih dahulu.

### Setelah Phase 5
Owner review KPI Builder.

Jika approved:
Lanjut Phase 6.

Jika revisi:
Perbaiki Phase 5 terlebih dahulu.

### Setelah Phase 6
Owner review Settings.

Jika approved:
Lanjut Phase 7.

Jika revisi:
Perbaiki Phase 6 terlebih dahulu.

### Setelah Phase 7
Prototype final siap digunakan untuk:
- Demo
- Validasi user
- Pitching
- Pengembangan backend lanjutan

---

## 11. Final Definition of Done

Prototype frontend dianggap selesai jika:

1. Landing page selesai.
2. Dashboard selesai.
3. KPI Tree page selesai.
4. KPI detail page selesai.
5. KPI builder prototype selesai.
6. Settings prototype selesai.
7. Semua halaman responsive.
8. Semua navigasi antar halaman berjalan.
9. Branding dark navy futuristic konsisten.
10. KPI Tree memperlihatkan hubungan sebab-akibat.
11. Dashboard tidak hanya menampilkan angka, tetapi juga insight.
12. Tidak ada backend/API/database.
13. Tidak ada fitur di luar scope.
14. Status fase terdokumentasi.
15. Prototype siap direview owner.

---

## 12. Current Project Status

### Status Umum
**Phase 0 — SOT Finalization: Pending Approval**

### Instruksi Saat Ini
Belum melakukan coding.

### Tindakan Berikutnya Setelah Approval
Jika owner menyetujui dokumen ini, eksekusi berikutnya adalah:

**Phase 1 — Build Landing Page Static HTML menggunakan HTML responsive + Tailwind CSS Play CDN native.**
