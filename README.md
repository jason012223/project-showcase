# 📂 Project Showcase — Jason Guijo

Case studies of the systems I've designed and shipped. Each entry is what the project **does**, what I **built**, and the **tech** behind it. Live links where available.

---

## 1. National CMMS Platform — *Vienovo* 🏭
**Production system · multi-plant maintenance management**

A computerized maintenance-management system for a national manufacturing operation. One dashboard where technicians, planners, and managers run work orders across multiple plants.

**What I built:**
- **Telegram field workflow** — technicians get assigned, accept/decline, log live progress, and sign off (photo-gated) directly in chat; every action syncs two-way with the web dashboard in real time. Supports multi-technician shared jobs.
- **Role-based access control** — server-enforced authorization, a configurable role/permission taxonomy (nothing hard-coded), break-glass super-admin recovery, and anti-corruption guards that prevent duplicate/ghost user records.
- **Multi-tier cost-approval engine** — approval chains that branch on cost thresholds, with emergency-bypass rules and a full audit trail.
- **Data-layer migration** — moved the source of truth off a fragile shared spreadsheet onto MongoDB, with a write-through mirror and an outage-fallback design so the system degrades gracefully.
- **SAP Goods-Issue integration** — auto-posts inventory movements on validation/approval.
- **Performance & reliability** — cut technician save latency from ~7s to ~1.1s; found and fixed a cache/circuit-breaker bug that was masking correct data in production.

**Tech:** TypeScript · Node.js/Express · React · MongoDB · Telegram Bot API · SAP · Azure · Vercel

> ⚠️ Source is proprietary to the employer. This is a description of my contribution, not a code release.

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

## 3. portfolio 🎨
**[Live](https://portfolio-lovat-ten-51.vercel.app) · [Repo](https://github.com/jason012223/portfolio)**

My personal portfolio site. Built with Next.js.

**Tech:** Next.js · CSS

---

## 4. VirtualArtGallery 🖼️
**[Repo](https://github.com/jason012223/VirtualArtGallery)**

A virtual art-gallery web experience.

**Tech:** JavaScript

---

### 📫 Contact
**jason.guijo2160@gmail.com** · Open to full-stack / backend roles
