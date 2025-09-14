# REBARA™ — Reinforced Concrete Design Assistant (MVP)

[![status](https://img.shields.io/badge/status-MVP-orange)](#)
[![improvements](https://img.shields.io/badge/state-UNDERGOING%20IMPROVEMENTS-blue)](#)
[![license](https://img.shields.io/badge/license-MIT-black)](#license)
[![PRs](https://img.shields.io/badge/PRs-welcome-brightgreen)](#contributing)
[![stack](https://img.shields.io/badge/stack-React%20%7C%20Tailwind%20%7C%20shadcn/ui%20%7C%20Framer%20Motion%20%7C%20pdfmake-informational)](#-tech-stack)

> **REBARA™** is a free, open, case-based learning and manual design tool for reinforced concrete, centered on **Eurocode 2** and **BS 8110**.  
> **This is the first repository of the MVP and is _currently undergoing improvements_.**

---

## ✨ What’s inside (MVP)
- **Design modules**:  
  **Column**, **Beam** (rectangular & flanged + span/depth proxy), **Slab**, **Foundation** (pad base with punching shear incl. interior/edge/corner & moment-transfer influence), **Staircase**.
- **Reports**: Print-optimised pages + **pdfmake** export (logo placeholder, **Table of Contents**, page footer: `project • date • REBARA™`).
- **Tutor Chat (RAG stub)**: `/tutor/answer` API spec, cites **clause identifiers** only.
- **AI Helpers**: Cost estimator, carbon footprint, tutorial prompts.
- **Codes**: **Eurocode 2 (EN 1992)** with UK NA, **BS 8110**. *(ACI 318, IS 456 — coming soon.)*

> **Disclaimer**: Educational tool only — **not a substitute for the Engineer of Record (EOR).**

---

## 🧭 Roadmap
- ✅ Mock calc flows for modules + report export  
- ✅ Punching shear: interior/edge/corner + moment transfer influence  
- 🔜 Clause-verified calc API (ULS/SLS, detailing)  
- 🔜 RAG backend (OpenAI embeddings + pgvector) & ingestion CLI  
- 🔜 NA parameter service; more codes (ACI 318, IS 456)  
- 🔜 Unit tests, accessibility pass, i18n, example projects

---

## 🖥 Tech Stack
**Frontend:** React, Tailwind CSS, shadcn/ui, Framer Motion  
**PDF:** pdfmake (client-side)  
**AI (planned):** OpenAI API + Postgres/pgvector (RAG)

---

## 🚀 Quick Start

### Prerequisites
- Node.js **18+** (LTS recommended)
- npm / pnpm / yarn

### Install & Run
```bash
git clone https://github.com/<your-org>/<repo>.git
cd <repo>
npm i
npm run dev
