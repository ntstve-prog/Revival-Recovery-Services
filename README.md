# Revival Recovery Services — Website Build

## Project Overview

**Revival Recovery Services** is a psychiatric mental health practice based in Surprise, Arizona, led by Conor Westerman, PMHNP-BC. This project builds a conversion-optimized, SEO-rich marketing website that positions the practice as the clear choice for psychiatric medication management and addiction recovery services in the Phoenix West Valley.

The current online presence is a barebones SimplePractice portal and a Psychology Today listing. This site replaces that with a professional, high-converting web presence that ranks, builds trust, and drives consultations.

---

## Tech Stack

- **Framework:** [Astro](https://astro.build/) (static-first, fast, SEO-native)
- **Styling:** Tailwind CSS v4
- **Animations:** CSS animations + Intersection Observer for scroll-triggered reveals
- **Forms:** Static HTML form with Netlify Forms / Formspree / or webhook to SimplePractice
- **Hosting:** Netlify or Vercel (static deploy)
- **Directory:** `developer/local-service-sites/revival-recovery/`

---

## Site Architecture

```
/                    → Home (primary landing + conversion page)
/about               → About Conor + Practice Philosophy
/contact             → "Free Consultation" Offer Page (NOT a generic contact page)
/terms               → Terms & Conditions
/privacy             → Privacy Policy
```

### Home Page Sections (scroll flow — single page funnel)

1. **Hero** — Emotionally resonant headline + subhead + primary CTA ("Schedule Your Free Consultation")
2. **Problem Agitation** — Speak to the pain: depression, addiction, feeling stuck, meds not working, overwhelming stress
3. **Solution / What We Do** — Medication management, MAT, recovery coaching, telehealth + in-person
4. **Why Revival** — Conor's differentiators: 13 years personal recovery, decade in mental health, Meadows BH experience, trauma-informed, evidence-based
5. **Services Breakdown** — Clean cards/sections for each service area with benefit-driven copy
6. **Insurance & Pricing** — Transparency builds trust. Show accepted insurance + cash rates
7. **Social Proof** — Endorsements from Psychology Today (Kelli Wagner LPC-S, Ernest Mall PMHNP)
8. **CTA / Offer Section** — "Are We the Right Fit?" → Free 15-min phone consultation capture form
9. **Footer** — Contact info, hours, links, emergency disclaimer

### About Page
- Conor's story: personal recovery journey, professional credentials, Meadows experience, Dr. Claudia Black mentorship
- Photo(s) of Conor
- Board certification details (PMHNP-BC, AZ License #227933)
- Philosophy: client-centered, collaborative, evidence-based, trauma-informed
- **Faith element:** Conor is a born-again Christian and his faith is part of his recovery story and whole-person approach. This should come through naturally in his personal narrative — not as branding, but as authenticity. Think: "My faith has been a cornerstone of my own recovery, and I believe in treating the whole person — mind, body, and spirit." It's woven into who he is, not a sales pitch. Patients of all backgrounds are welcome. The tone is inclusive and grounded, not preachy. This positions him for clients who value a provider with spiritual depth without alienating anyone who doesn't.

### Contact / Offer Page
- **This is NOT a contact page. This is a conversion page.**
- Headline: Offer-framed (e.g., "Your First Step Costs Nothing — Schedule a Free 15-Minute Consultation")
- Short qualifying copy: who this is for, what to expect
- Form fields: Name, Phone, Email, "What brings you in?" (dropdown: Depression, ADHD, Addiction/Recovery, Trauma/PTSD, Medication Review, Other), Preferred contact method, Insurance provider
- Secondary CTA: Direct call link (928) 588-6413 / text (623) 670-3622
- Trust badges: Licensed in AZ, accepts insurance, telehealth available

---

## Content Constraints

**IMPORTANT: The word "anxiety" must NOT appear anywhere on the site.** This is a client directive. Do not use it in headlines, body copy, service lists, meta descriptions, keywords, schema markup, alt tags, or anywhere else. Where the concept would naturally come up, use alternatives like "stress," "overwhelming thoughts," "mental health challenges," or simply omit it. This applies to all pages and all code.

---

## Design Direction

### Aesthetic: "Refined Recovery" — Clean, warm, grounded luxury

Think: high-end wellness brand meets clinical credibility. Not sterile medical. Not woo-woo wellness. The intersection of professional trust and human warmth.

- **Color Palette:**
  - Deep navy/slate (`#1a2332`) — authority, trust
  - Warm sand/cream (`#f5f0e8`) — approachable, calming
  - Muted sage green (`#7a9e7e`) — growth, renewal, recovery
  - Accent: warm amber/copper (`#c4854c`) — energy, warmth, hope
  - Text: rich charcoal (`#2d2d2d`) on light, warm white (`#fafaf7`) on dark

- **Typography:**
  - Display/Headlines: A distinctive serif — something like `DM Serif Display`, `Playfair Display`, or `Lora` (classic, trustworthy, warm)
  - Body: Clean humanist sans — `DM Sans`, `Source Sans 3`, or `Outfit` (readable, modern, approachable)
  - Avoid: Inter, Roboto, Arial, anything generic

- **Visual Language:**
  - Generous whitespace — let the content breathe
  - Subtle texture: light linen/paper grain on backgrounds
  - Organic shapes: soft rounded sections, gentle curves
  - Photography: Use Conor's actual photos (warm, professional, real)
  - Subtle scroll-triggered fade-ins and slide-ups
  - NO stock photos of fake smiling people. NO generic medical imagery.

- **Mobile First:** 70%+ of mental health searches are mobile. Every section must feel native on a phone.

---

## SEO Strategy

### Primary Keywords (target in title tags, H1s, meta descriptions, body copy)
- `psychiatric nurse practitioner surprise az`
- `medication management surprise arizona`
- `PMHNP surprise az`
- `mental health medication management phoenix`
- `addiction recovery surprise arizona`
- `MAT medication assisted treatment surprise az`
- `depression medication surprise az`
- `psychiatric services west valley az`
- `telehealth psychiatry arizona`

### Secondary / Long-tail Keywords
- `ADHD medication management surprise az`
- `bipolar disorder treatment surprise arizona`
- `substance abuse treatment surprise az`
- `suboxone provider surprise az`
- `mental health prescriber near me`
- `psychiatric nurse practitioner accepting insurance arizona`
- `online psychiatry arizona`
- `depression medication prescriber phoenix west valley`
- `stress and mental health treatment surprise az`

### Local SEO Signals
- NAP consistency: **Revival Recovery Services** | Surprise, AZ 85387 | (928) 588-6413
- Secondary location mention: 4527 N 16th St, Phoenix, AZ 85016
- Schema markup: `MedicalBusiness`, `Physician`, `LocalBusiness`
- Service area pages potential: Surprise, Glendale, Peoria, Sun City, Buckeye, Goodyear, Phoenix West Valley

### Technical SEO
- Semantic HTML5 throughout
- Proper heading hierarchy (single H1 per page, structured H2-H4)
- Meta titles: `[Primary Keyword] | Revival Recovery Services — Surprise, AZ`
- Meta descriptions: Benefit-driven, include CTA, 150-160 chars
- Open Graph + Twitter Card meta for social sharing
- JSON-LD structured data for LocalBusiness + MedicalBusiness
- Sitemap.xml + robots.txt
- Image alt tags with keyword context
- Core Web Vitals optimized (Astro handles this well out of the box)
- Canonical URLs on every page

---

## Conversion Strategy

Every page has ONE job: move the visitor toward scheduling that free consultation.

### Funnel Logic
```
Visitor lands (SEO / Google Maps / referral)
    ↓
Hero creates emotional connection + immediate CTA
    ↓
Problem section validates their pain ("you're not alone, this is fixable")
    ↓
Solution section positions Revival as the answer
    ↓
Credibility section removes doubt (credentials, recovery story, endorsements)
    ↓
Offer section removes friction ("free, 15 minutes, no commitment")
    ↓
Form capture → lead → appointment
```

### CTA Strategy
- **Primary CTA:** "Schedule Your Free Consultation" (appears 3-4x on homepage)
- **Secondary CTA:** "Call Now" with click-to-call
- **Tertiary CTA:** "Text Us" for the phone-call-averse crowd
- Sticky mobile CTA bar at bottom of screen
- Every section ends with a micro-CTA or transition to next section

### Trust Signals
- "Verified by Psychology Today" badge
- "Licensed in Arizona — #227933"
- Insurance logos/names
- Endorsement quotes from named, credentialed professionals
- "13 Years in Personal Recovery" — authenticity is the ultimate trust signal
- "Trained at The Meadows Behavioral Healthcare"
- "Telehealth & In-Person Available"

---

## Practice Details (Source of Truth)

### Provider
- **Name:** Conor Westerman
- **Credentials:** PMHNP-BC (Psychiatric Mental Health Nurse Practitioner — Board Certified)
- **License:** Arizona #227933
- **NPI:** (verify with Conor)
- **Experience:** 10+ years in mental health, PMHNP-BC earned 2024
- **Personal:** 13+ years in recovery

### Contact
- **Phone (PT listing):** (928) 588-6413
- **Phone (SimplePractice):** (623) 670-3622
- **Email:** Conor.westermanrecovery@gmail.com
- **Client Portal:** https://conor-westerman.clientsecure.me/

### Locations
- **Primary:** Surprise, AZ 85387 (telehealth)
- **Secondary/In-Person:** 4527 N 16th St, Phoenix, AZ 85016

### Services
- Psychiatric Medication Management
- Medication-Assisted Treatment (MAT) for Addiction
- Recovery Coaching
- Crisis Intervention
- Psychiatric Consultations
- Telehealth & In-Person Available

### Conditions Treated
- Depression
- PTSD / Trauma
- ADHD / ADD
- Bipolar Disorder
- Substance Use / Addiction
- Alcohol Use Disorder
- Eating Disorders
- Borderline Personality Disorder
- Chronic Relapse
- Dual Diagnosis
- Suicidal Ideation
- Anger Management
- Family Conflict
- Stress

### Treatment Approaches
- Trauma-Informed Care
- Cognitive Behavioral (CBT)
- Dialectical Behavior (DBT)
- Motivational Interviewing
- 12-Step Friendly
- Person-Centered
- Positive Psychology
- Ketamine-Assisted (verify current status)
- Faith-informed / whole-person approach (not listed as "Christian Counseling" — frame as treating mind, body, and spirit)

### Insurance Accepted
- Aetna
- Blue Cross Blue Shield of Arizona
- Cigna / Evernorth
- UnitedHealthcare / UHC / UBH
- Optum
- Oscar Health
- Oxford
- United Medical Resources (UMR)
- Carelon Behavioral Health
- Quest Behavioral Health

### Pricing
- Initial Session: $200
- Follow-Up: $100
- Sliding scale available
- Payment: ACH, Amex, Apple Cash, Cash, Check, PayPal, Venmo, Visa, Zelle

### Client Focus
- Ages: Children (6+), Teens, Adults, Elders (65+)
- Individuals, Families, Groups

### Endorsements (from Psychology Today)
1. **Kelli Wagner, LPC-S, CSAT** — "Conor is a very skilled and compassionate provider. I had the pleasure of working with him at The Meadows Behavioral Health over a number of years and highly recommend his services."
2. **Ernest Mall, PMHNP-BC** — "Professional and compassionate provider, follows evidence based practices and provides great client care."

---

## File Structure

```
revival-recovery/
├── public/
│   ├── fonts/
│   ├── images/
│   │   ├── conor-headshot.jpg      ← need from client
│   │   ├── conor-secondary.jpg     ← need from client
│   │   └── og-image.jpg            ← generate for social
│   ├── favicon.svg
│   ├── robots.txt
│   └── sitemap.xml                 ← auto-generated by Astro
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── ProblemSection.astro
│   │   ├── ServicesSection.astro
│   │   ├── AboutPreview.astro
│   │   ├── InsuranceSection.astro
│   │   ├── TestimonialsSection.astro
│   │   ├── CTASection.astro
│   │   ├── ConsultationForm.astro
│   │   ├── MobileCTABar.astro
│   │   └── SchemaMarkup.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   ├── about.astro
│   │   ├── contact.astro
│   │   ├── terms.astro
│   │   └── privacy.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── tailwind.config.mjs
├── package.json
├── tsconfig.json
└── README.md
```

---

## Assets Needed from Client

- [ ] High-res headshot (current one from Psychology Today works as fallback)
- [ ] Secondary photo (in clinical setting or casual professional)
- [ ] Confirm which phone number is primary for the website
- [ ] Confirm if Ketamine-Assisted is an active offering
- [ ] Logo file if one exists (otherwise we design a wordmark)
- [ ] Confirm business hours / availability windows
- [ ] Google Business Profile access for NAP consistency audit

---

## Deployment Notes

- Static build via `astro build` → deploy to Netlify/Vercel
- Form submissions route to email or webhook
- SSL certificate (auto via hosting)
- Set up Google Search Console + submit sitemap post-launch
- Connect Google Analytics 4
- Verify/claim Google Business Profile and link to new site


