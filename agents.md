# AGENTS.md
## KPI Builder untuk UMKM — SOT-Driven Frontend Agent Instruction

---

## 1. Agent Role

You are a modern frontend developer, system analyst, UX designer, and implementation agent for the **KPI Builder untuk UMKM** project.

Your job is to implement the frontend prototype based strictly on the Single Source of Truth documents in the `/docs` folder:

1. `docs/PRD.md`
2. `docs/UI-Guidelines.md`
3. `docs/Implementation-Plan.md`

You must not improvise beyond the approved scope.

---

## 2. Project Goal

Build a static frontend prototype for **KPI Builder untuk UMKM**, consisting of:

1. Landing Page / Company Profile
2. Main KPI Dashboard
3. KPI Tree View
4. KPI Detail View
5. KPI Builder Prototype
6. Settings Prototype

The dashboard must clearly show the **cause-effect relationship between KPIs** and must make the **KPI Tree** easy to understand.

---

## 3. Required Tech Stack

Use only:

- Native HTML
- Tailwind CSS Play CDN
- Lightweight vanilla JavaScript only if needed for dummy interactions
- Static dummy data
- File-based pages

Do not use:

- React
- Next.js
- Vue
- Angular
- Backend
- Database
- Authentication
- Payment gateway
- API integration
- NPM packages
- Build tools
- External chart libraries

---

## 4. Visual Direction

Follow the UI Guidelines exactly.

Design style:

**Dark Navy Futuristic, Clean SaaS, Millennial–Gen Z Modern, Professional Consulting Tech.**

The interface must feel:

- Modern
- Strategic
- Futuristic
- Clean
- Business-friendly
- UMKM-friendly
- Professional but not stiff

Main visual colors:

- Dark navy / slate background
- Electric blue / cyan accent
- Indigo / violet supporting gradient
- Green / amber / red semantic KPI status colors

---

## 5. Mandatory File Structure

Create the project using this structure:

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
├── agents.md
└── README.md
```

If the repository already contains the `/docs` folder and `agents.md`, keep them and do not delete them.

---

## 6. Implementation Phases

You must work phase by phase.

### Phase 0 — Read and Confirm SOT

Before coding:

1. Read `PRD.md`.
2. Read `UI-Guidelines.md`.
3. Read `Implementation-Plan.md`.
4. Summarize your understanding.
5. Confirm the next implementation phase.

Do not start coding until the owner gives approval.

---

### Phase 1 — Landing Page

Deliverable:

- `index.html`

Build:

1. Navbar
2. Hero section
3. Problem section
4. Solution section
5. Feature section
6. KPI Tree explanation section
7. Dashboard preview section
8. Use case section
9. Pricing placeholder
10. FAQ
11. CTA
12. Footer

Rules:

- Use Tailwind Play CDN.
- Use responsive layout.
- CTA “Coba Dashboard” must link to `dashboard.html`.
- The landing page must sell the value of KPI cause-effect and KPI Tree.
- Stop after Phase 1 and report completion.

---

### Phase 2 — Main Dashboard

Deliverable:

- `dashboard.html`

Build:

1. App topbar
2. Dashboard header
3. Dummy filters
4. Business Health Score panel
5. KPI summary cards
6. KPI Tree preview
7. Cause-effect insight panel
8. Risk alert section
9. Recommended action section
10. KPI table summary

Rules:

- Dashboard must not be just a generic admin template.
- The relationship between KPI drivers and outcome KPIs must be visible.
- Use dummy data consistently.
- Stop after Phase 2 and report completion.

---

### Phase 3 — KPI Tree Page

Deliverable:

- `kpi-tree.html`

Build:

1. Page header
2. Strategic Objective node
3. Outcome KPI node
4. Business Driver KPI nodes
5. Operational KPI nodes
6. Action Indicator nodes
7. Connection lines / arrows
8. Legend
9. Selected KPI side panel

Rules:

- The KPI Tree must show cause-effect hierarchy clearly.
- Direction should show drivers leading to outcomes.
- KPI statuses must be visible through badges and labels.
- Mobile layout must remain usable.
- Stop after Phase 3 and report completion.

---

### Phase 4 — KPI Detail Page

Deliverable:

- `kpi-detail.html`

Build:

1. KPI header
2. Status summary
3. Formula section
4. Target vs actual section
5. Owner and review frequency
6. Upstream drivers
7. Downstream impacts
8. Risk explanation
9. Recommended action

Rules:

- KPI detail must explain why the KPI matters.
- Show upstream cause and downstream impact clearly.
- Stop after Phase 4 and report completion.

---

### Phase 5 — KPI Builder Prototype

Deliverable:

- `builder.html`

Build:

1. Business goal input
2. Business type selector
3. Function area selector
4. KPI type selector
5. KPI name input
6. Formula input
7. Target input
8. Parent KPI selector
9. KPI card preview
10. KPI Tree position preview

Rules:

- No real form submission is required.
- This is a static prototype.
- The user must understand how a KPI is connected to a parent KPI.
- Stop after Phase 5 and report completion.

---

### Phase 6 — Settings Prototype

Deliverable:

- `settings.html`

Build:

1. Business profile section
2. KPI category setting
3. Review period setting
4. Team/function placeholder
5. Export setting placeholder

Rules:

- This is only a visual placeholder.
- No backend or save function.
- Stop after Phase 6 and report completion.

---

### Phase 7 — QA and Polish

Deliverable:

- Final static prototype

Check:

1. Desktop responsiveness
2. Tablet responsiveness
3. Mobile responsiveness
4. Navigation links
5. Visual consistency
6. KPI Tree clarity
7. Dashboard hierarchy
8. Typography readability
9. CTA visibility
10. No backend/API/database usage

Stop after Phase 7 and report final completion.

---

## 7. Dummy KPI Data Standard

Use this business context:

- Business name: UMKM Demo
- Industry: Retail & F&B
- Period: Juni 2026
- Main objective: Meningkatkan Profitabilitas Bisnis

Use these KPI examples:

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
11. Marketing Cost Ratio
12. Inventory Waste
13. Sales Follow-Up Rate
14. Promo Effectiveness
15. Stock Accuracy
16. Supplier Cost Control

KPI status types:

- Healthy
- Watch
- Critical

KPI hierarchy types:

- Strategic Objective
- Outcome KPI
- Driver KPI
- Operational KPI
- Activity Indicator

---

## 8. KPI Tree Logic

The KPI Tree must follow this logic:

```text
Strategic Objective
└── Outcome KPI
    ├── Business Driver KPI
    │   ├── Operational KPI
    │   │   └── Activity Indicator
```

Example:

```text
Meningkatkan Profitabilitas Bisnis
└── Net Profit Margin
    ├── Revenue Growth
    │   ├── Conversion Rate
    │   ├── Average Transaction Value
    │   └── Repeat Purchase Rate
    ├── Gross Margin
    │   ├── COGS Ratio
    │   ├── Inventory Waste
    │   └── Supplier Cost Control
    └── Operating Cost Ratio
        ├── Marketing Cost Ratio
        └── Service Response Time
```

The UI must communicate that:

- Operational KPIs drive Business Driver KPIs.
- Business Driver KPIs affect Outcome KPIs.
- Outcome KPIs determine strategic objective achievement.

---

## 9. Copywriting Rules

Use Indonesian language.

Tone:

- Clear
- Practical
- Strategic
- Friendly for UMKM owners
- Professional enough for consultants

Avoid:

- Overly academic language
- Overly technical terms without explanation
- Long paragraphs
- Claims that guarantee profit
- Generic SaaS copy that does not mention KPI Tree or cause-effect logic

Good examples:

- “Jangan hanya pantau angka. Pahami penyebabnya.”
- “Lihat KPI mana yang benar-benar mendorong profit.”
- “Hubungkan target bisnis dengan aktivitas harian tim.”
- “Temukan akar masalah sebelum mengambil keputusan.”

---

## 10. Quality Bar

The implementation is acceptable only if:

1. It follows the SOT documents.
2. It uses only HTML + Tailwind Play CDN.
3. It is responsive.
4. It has a premium dark navy futuristic style.
5. It clearly shows KPI cause-effect logic.
6. It includes a visible KPI Tree.
7. It does not use backend, database, auth, or API.
8. It does not add unapproved features.
9. It has clear navigation between pages.
10. It stops at each phase for owner approval.

---

## 11. Critical Constraints

Do not:

- Replace the KPI Tree with generic charts.
- Build a normal admin dashboard without cause-effect logic.
- Add complex dependencies.
- Add backend logic.
- Add fake login logic.
- Add payment integration.
- Add AI API calls.
- Add pages outside the approved structure.
- Change the design direction.
- Delete SOT documents.

---

## 12. First Instruction for Codex

Start by reading all SOT documents.

Then respond with:

1. Summary of the product goal.
2. Summary of the UI direction.
3. Summary of the implementation constraints.
4. Confirmation that no code will be created before Phase 1 approval.
5. Ask for approval to start Phase 1.

Only after explicit approval, build `index.html` for Phase 1.
