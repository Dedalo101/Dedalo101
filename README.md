# Dedalo101

**Independent music label · artist platform · performance-first web architecture**

Dedalo101 builds and operates the digital infrastructure behind [Glue Records](https://gluerecords.club) — an underground electronic music label operating between Málaga (ES) and Amsterdam (NL). We ship fast, static, GDPR-aware artist sites and shared tooling that scales the roster without scaling headcount.

---

## What we do

| Pillar | Description |
|--------|-------------|
| **Glue Records** | Label roster, releases, bookings, live events — [gluerecords.club](https://gluerecords.club) |
| **Artist sites** | One repo per artist; shared `Dedalo101-Core` architecture, unique visual identity |
| **Platform tooling** | Site bootstrap, SEO injection, Cloudflare Pages deploy, Formspree bookings |
| **Dedalus-Converger** | Constraint-based infra reconciliation engine (proprietary) |

---

## Roster (live sites)

| Artist | Site | Stack |
|--------|------|-------|
| Nahuel | [nahuel.club](https://nahuel.club) | Static · GitHub Pages |
| Edomite | [edomite.club](https://edomite.club) | Static · Cloudflare Pages |
| Amoro | [amoro.club](https://amoro.club) | Static · GitHub Pages |
| Kamaleonica | [kamaleonica.com](https://kamaleonica.com) | Static · GitHub Pages |
| Benny Yasoto | [bennyasoto.com](https://bennyasoto.com) | Static · Cloudflare Pages |
| Breaking Robots | [breakingrobots.com](https://breakingrobots.com) | React/Vite · Cloudflare |
| DJ Hoppi | [djhoppi.club](https://djhoppi.club) | Static · GitHub Pages |
| Prisss | [prisss.com](https://prisss.com) | Static · Formspree bookings |

---

## Engineering principles

- **Performance first** — Core Web Vitals targets; homepage under 2 MB; WebP + lazy loading
- **Privacy by design** — No tracking without consent; Formspree for contact data; PII never in git ([PRIVACY.md](https://github.com/Dedalo101/Dedalo101-Core/blob/main/PRIVACY.md))
- **Trunk-based delivery** — `main` is deployable; CI on every artist repo; secrets via GitHub Actions only
- **Shared core, free aesthetics** — [`Dedalo101-Core`](https://github.com/Dedalo101/Dedalo101-Core) components + per-artist `theme.css`

Full standards: [CONTRIBUTING.md](https://github.com/Dedalo101/Dedalo101-Core/blob/main/CONTRIBUTING.md) · [SECURITY.md](https://github.com/Dedalo101/Dedalo101-Core/blob/main/SECURITY.md)

---

## Key repositories

| Repo | Role |
|------|------|
| [GlueRecords](https://github.com/Dedalo101/GlueRecords) | Label hub site |
| [Dedalo101-Core](https://github.com/Dedalo101/Dedalo101-Core) | Shared architecture, scripts, compliance docs |
| [Dedalus-Converger](https://github.com/Dedalo101/Dedalus-Converger) | Infra reconciliation (proprietary) |
| [dedalo-pocketbase-dart](https://github.com/Dedalo101/dedalo-pocketbase-dart) | Artist platform SDK (Dart) |

---

## Data protection (GDPR)

Dedalo101 processes personal data only where necessary for bookings, newsletters, and site analytics — with explicit consent where required by EU law.

- **Controller contact:** [info@gluerecords.club](mailto:info@gluerecords.club)
- **Policy:** [PRIVACY.md](https://github.com/Dedalo101/Dedalo101-Core/blob/main/PRIVACY.md)
- **Practices:** No customer/RA export CSVs in repositories; `.gitignore` blocks PII paths; Formspree as processor for booking forms

---

## Contact

- **Label & bookings:** [info@gluerecords.club](mailto:info@gluerecords.club)
- **GitHub:** [@Dedalo101](https://github.com/Dedalo101)
- **Label site:** [gluerecords.club](https://gluerecords.club)

---

*© 2024–2026 Dedalo101 · Glue Records. Proprietary assets where noted; open components under MIT in Dedalo101-Core.*
