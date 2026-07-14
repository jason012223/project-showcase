# 📂 Project Showcase — Jason Guijo

Case studies of the systems I've designed and shipped. Each entry is what the project **does**, what I **built**, and the **tech** behind it. Live links where available.

---

## 1. National CMMS Platform 🏭
**Production system · multi-plant maintenance management · client project (proprietary)**

A computerized maintenance-management system for a national manufacturing operation. One dashboard where technicians, planners, and managers run work orders across multiple plants.

**What I built:**
- **Telegram field workflow** — technicians get assigned, accept/decline, log live progress, and sign off (photo-gated) directly in chat; every action syncs two-way with the web dashboard in real time. Supports multi-technician shared jobs.
- **Role-based access control** — server-enforced authorization, a configurable role/permission taxonomy (nothing hard-coded), break-glass super-admin recovery, and anti-corruption guards that prevent duplicate/ghost user records.
- **Multi-tier cost-approval engine** — approval chains that branch on cost thresholds, with emergency-bypass rules and a full audit trail.
- **Data-layer migration** — moved the source of truth off a fragile shared spreadsheet onto MongoDB, with a write-through mirror and an outage-fallback design so the system degrades gracefully.
- **SAP Goods-Issue integration** — auto-posts inventory movements on validation/approval.
- **Performance & reliability** — cut technician save latency from ~7s to ~1.1s; found and fixed a cache/circuit-breaker bug masking correct data in production.

**Tech:** TypeScript · Node.js/Express · React · MongoDB · Telegram Bot API · SAP · Azure · Vercel

> ⚠️ Client source is proprietary. This is a description of my contribution, not a code release.

---

## 2. chromabooth 📸
**[Live](https://chromabooth.vercel.app) · [Repo](https://github.com/jason012223/chromabooth)**

A Y2K chrome-metallic photobooth in the browser.

- Live camera viewfinder (mirrored preview, non-mirrored exports)
- 8 real-time AR filters rendered on canvas
- Drag-and-drop stickers, 6 photo layouts, 4 frame templates, baked on capture
- Countdown timer, capture flash, client-side PNG strip download
- Optional backend: cloud sessions, strip compositing, QR + email delivery
- PWA baseline (installable, offline app-shell)

**Tech:** React · WebRTC · Canvas · Zustand · Node/Express · Prisma · Cloudinary · Sharp · Resend

---

## 3. Y2K Editorial Booth 💿
Browser-based photobooth concept focused on real-time Y2K face stickers, live camera filters, and polished editorial exports. Uses on-device face-landmark tracking for sticker placement.

**Tech:** React · MediaPipe (face landmarks) · GSAP · Framer Motion · OGL

---

## 4. BudgetTracker 📊
Offline-first personal budget tracker built for the Philippines. Native Android — one-time-purchase core, with cloud + bank sync planned as a v2 add-on.

**Tech:** Kotlin · Jetpack Compose · Android

---

## 5. Trading System 📈
Honest backtesting and signal engine for US stocks and forex — built to test strategies without lookahead bias or curve-fit optimism.

**Tech:** Python

---

## 6. agentic-os 🤖
A personal AI-assisted development hub that ties together code knowledge graphs and a project-memory vault, so an AI assistant is oriented on each project automatically.

**Tech:** Python · knowledge graphs · local tooling

---

## 7. Virtual Art Gallery 🖼️
**[Repo](https://github.com/jason012223/VirtualArtGallery)**

A museum rendered in 3D that you walk through in first-person. Joystick / on-screen controls for movement and look, so visitors roam the halls and view the exhibits from any angle — a virtual gallery in the browser.

**Tech:** Three.js · WebGL · JavaScript

---

## 8. IT Operations Dashboard 🖥️
**Internal tool · organization deployment**

An internal IT-operations dashboard for managing helpdesk tickets, assets, network monitoring, and purchasing from one place.

**Tech:** Next.js · React · Prisma · PostgreSQL

---

## 9. Forms & Approval-Workflow System 📝
**Internal tool · organization deployment**

An internal request-and-approval platform: employees submit requests (cash advances, reimbursements, travel bookings, custom forms), approvers act on them, processors finalize, and admins manage form definitions, users, roles, and settings.

**Tech:** Next.js · MongoDB (Mongoose) · Firebase

> ⚠️ Built for an employer — this describes my contribution, not a code release.

---

## 10. SCADA → ERP Integration ⚙️
**Internal tool · industrial data pipeline (confidential client)**

An integration service that pulls production and consumption data from an industrial SCADA supervisory layer and posts it automatically into an ERP (SAP Business One) — turning shop-floor telemetry into accurate inventory/consumption records without manual re-keying.

**Tech:** C# / .NET · SAP Business One · SCADA data sources

> ⚠️ Confidential client engagement — capability described only; no client identity, data, or source.

---

## 11. Certificate-Issuance Workflow Portal 📜
**Internal tool · regulated document workflow (confidential client)**

A portal that runs a certificate-issuance process end-to-end: applicants submit requests, reviewers and approvers act in sequence, and approved certificates are generated as documents and delivered by email — with role-based access and an auditable workflow throughout.

**Tech:** Next.js · NestJS · MongoDB · Redis (job queue) · object storage · JWT auth (pnpm monorepo)

> ⚠️ Confidential client engagement — capability described only; no client identity, data, or source.

---

### 📫 Contact
**jason.guijo2160@gmail.com** · Open to full-stack / backend roles
