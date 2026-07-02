# Webyor — Project Showcase

**Live site:** [webyor.com](https://webyor.com)

> A custom-built agency website for **Webyor**, a software development studio for founders and businesses. This README is a **portfolio/interview reference** — it documents the architecture, stack, and strategy behind the project without exposing any source code, as the codebase is private.

---

##  What This Project Is

Webyor's official agency website — built to prove the studio's engineering standard through the site itself, not through a sales pitch. The brief was: premium visual design, strong performance, and SEO/AIO readiness baked in from the start, so the site functions as a live demonstration of the kind of work the agency does.

- **Type:** Agency website / technical showcase (UI, performance, SEO & AIO focus)
- **Role:** End-to-end design + development
- **Status:** Live in production

---

##  Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js 16 (App Router) |
| UI Library | React 19 |
| Language | TypeScript |
| Styling | Vanilla CSS — custom design system, glassmorphism, dark-mode aesthetics |
| Animation | Framer Motion (declarative UI animation) + GSAP (timeline-based sequencing) |
| 3D Graphics | Three.js |
| Icons | Lucide React |
| Email/Forms | Resend |
| Analytics | Vercel Analytics |
| Hosting | Vercel |

---

##  Key Engineering Highlights

- **Premium, dynamic UI** — vibrant color system, dark mode, and glassmorphism used deliberately rather than templated defaults.
- **Micro-interactions & scroll-reveals** — subtle motion design throughout the page to guide attention without feeling gimmicky.
- **Immersive 3D elements** — custom Three.js scenes integrated into the hero/landing experience.
- **Performance-first build** — tuned for strong Core Web Vitals and fast Largest Contentful Paint (LCP), despite the animation and 3D-heavy front end.
- **Reusable component architecture** — scalable, composable components rather than one-off page code.

---

##  SEO & AIO (AI Optimization) Strategy

Built to be legible to both search engines and AI crawlers/answer engines:

- **Structured data (JSON-LD)** for Organization, Person, and WebSite schemas, powering rich snippets.
- **Dynamic, auto-generated sitemap** for efficient crawling.
- **Rigorous semantic HTML** — proper heading hierarchy (`h1`–`h6`), unique IDs, accessible markup.
- **Fully optimized meta tags & Open Graph data** for every route, dynamically generated.
- **Server-rendered content via Next.js** — pages ship complete HTML rather than a blank shell that depends on client-side JS, which is significantly easier for both traditional search bots and LLM-based crawlers to parse and summarize.

This mirrors the "Technical SEO, AIO & Growth" service the agency itself offers — the site is effectively a live case study of that service.

---

##  Performance & Core Web Vitals

Verified via [Google PageSpeed Insights](https://pagespeed.web.dev/) (Desktop):

| Category | Score |
|---|---|
| Performance | **100** |
| Accessibility | 96 |
| Best Practices | **100** |
| SEO | **100** |

| Metric | Value |
|---|---|
| First Contentful Paint (FCP) | 0.3 s |
| Largest Contentful Paint (LCP) | 0.7 s |
| Total Blocking Time (TBT) | 20 ms |
| Cumulative Layout Shift (CLS) | 0 |
| Speed Index | 0.9 s |

A perfect Performance score with sub-second LCP is notable given the site runs Framer Motion, GSAP, and Three.js on the front end — it reflects deliberate optimization work (server rendering, careful animation scoping, asset/loading discipline) rather than a lightweight page getting a free pass.

---

##  Core Site Sections

- **Hero** — value proposition, dual CTA (Book a Discovery Call / WhatsApp)
- **Trust strip** — direct engineer access, fixed pricing, lifetime bug-fix guarantee
- **Manifesto** — scroll-driven narrative section
- **Services** — Web Applications, Mobile App Development (React Native), Performance & Optimization, Technical SEO/AIO & Growth
- **Why Webyor** — value propositions (Ship Fast, Own Everything, Stay Accountable, Fix It for Life)
- **FAQ** — an extensive, structured Q&A knowledge base covering custom software, web/mobile development, React/Next.js, .NET, Azure, API integration, and business automation — written to double as AIO-friendly long-form content
- **Contact** — booking, WhatsApp, and email-based contact options

---

##  Deployment

- Domain purchased, configured, and deployed end-to-end (DNS, hosting, SSL) by me
- Deployed on Vercel with a custom domain (webyor.com)
- Production-ready for Google Search Console submission and rapid indexing

---

##  A Note on Source Code

This repository/README exists specifically so the project can be discussed and demonstrated (architecture, decisions, stack, strategy) **without publishing the underlying codebase**. Happy to walk through implementation details, trade-offs, or specific technical decisions in conversation — just not the raw source.
