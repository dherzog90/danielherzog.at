# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **private portfolio website** for Daniel Herzog, a Software Architect based in Austria. The site is a single-page application built with vanilla HTML, CSS (Tailwind), and JavaScript.

**Important Legal Positioning:**
- This is a **private portfolio site** (NOT a commercial website)
- Purpose: Showcase professional qualifications, skills, and certifications
- Does NOT offer commercial services or products
- Uses simplified imprint requirements per § 25 Abs. 5 Austrian Media Law (Mediengesetz)

## Architecture

**Single-File Structure:**
- `index.html` - Complete website in a single HTML file containing all sections, styles, and scripts
- No build process or dependencies - runs directly in browser
- Uses Tailwind CSS via CDN (not npm)

**Content Language:**
- The website is in **German** (lang="de")
- All user-facing content must be in German
- Contact information: danielherzog@outlook.com, +43 664 17 34 963

**Sections:**
1. Hero - Professional title and introduction
2. Kompetenzen (Skills) - Technical skills showcase focused on:
   - Software Architecture (Enterprise, Microservices, Cloud, Design Patterns)
   - Software Development (Full-Stack, API Design, Code Review, Agile)
   - Cloud & AI (Azure, Azure AI, KI-Integration, DevOps)
   - Technical Expertise highlights (certifications)
3. Erfahrung (Experience) - Education and certifications
4. Kontakt (Contact) - Contact form for non-commercial purposes (networking, professional exchange)
5. Footer - Copyright, imprint link, and private portfolio disclaimer

**Design System:**
- Primary color: `#2563eb` (blue)
- Secondary color: `#1e40af` (darker blue)
- Responsive design with mobile menu
- Smooth scroll navigation
- Gradient backgrounds: `from-blue-50 to-indigo-100` and `from-blue-600 to-indigo-700`

## Key Implementation Details

**Contact Form:**
- Uses `mailto:` link instead of backend
- Opens user's email client with pre-filled subject and body
- Form fields: name, email, message

**Certifications to Display:**
1. Microsoft Certified: Azure AI Fundamentals (April 2024)
2. KI-KOMPETENZTRAINING nach Art. 4 AI Act (August 2025)
3. Certified Professional for Software Architecture (January 2017)
4. Certified Professional for Requirements Engineering (January 2014)

**Professional Focus:**
- Emphasize technical skills over management/leadership
- Position as Software Architect (personal portfolio, NOT service offering)
- Highlight certifications in Software Architecture, Requirements Engineering, and Azure AI
- All content focuses on showcasing qualifications, NOT selling services

## Making Changes

Since this is a static HTML file with no build process:
- Edit `index.html` directly
- Test by opening the file in a browser
- All Tailwind classes are available via CDN
- JavaScript is inline in the `<script>` tag at the bottom

**Navigation:**
- Uses anchor links (`#home`, `#about`, `#experience`, `#contact`)
- Mobile menu toggles visibility with JavaScript
- Smooth scroll enabled via `scroll-smooth` class on `<html>`

**Animation:**
- Sections fade in on scroll using IntersectionObserver
- Initial opacity: 0, transform: translateY(20px)
- Animates to opacity: 1, transform: translateY(0)

## Legal & Imprint Information

**Website Type:**
- Private portfolio website (non-commercial)
- Austrian law applies (Mediengesetz § 25 Abs. 5)
- Hosted on Cloudflare

**Imprint (impressum.html):**
- Minimal imprint per § 25 Abs. 5 Media Law
- Contains: Name (Daniel Herzog) and location (Lengenfeld, Austria)
- Does NOT contain: Business registration, VAT number, company form (not required for private sites)
- Includes basic contact information (email, LinkedIn)
- Clearly states: "Private Portfolio-Seite" (private portfolio site)

**Footer Disclaimers:**
Both `index.html` and `impressum.html` contain footer disclaimers stating:
- "Dies ist eine private Portfolio-Seite zur Darstellung meiner Fähigkeiten und Qualifikationen."
- "Diese Website dient nicht kommerziellen Zwecken."
- Located in footer: Small text (`text-xs`, `text-gray-500`)

**Contact Section:**
- Explicitly states: "für nicht-kommerzielle Zwecke" (for non-commercial purposes)
- Purpose: Professional exchange, networking, general inquiries
- Uses mailto: link (no backend processing)

**Privacy & Analytics:**
- Uses Cloudflare Web Analytics (GDPR-compliant)
- Cloudflare Web Analytics is:
  - Cookie-free
  - Does not collect personal data
  - Does not collect IP addresses
  - Does not enable cross-site tracking
- Analytics script is automatically injected by Cloudflare during deployment (no manual script insertion needed)
- Privacy information documented in impressum.html (Datenschutz section)

**Important Note:**
If this website is ever used to receive paid work or offer commercial services, it MUST be converted to a commercial site with:
1. Business registration (Gewerbeanmeldung)
2. Full commercial imprint with all required legal information
3. Removal of "private portfolio" disclaimers
