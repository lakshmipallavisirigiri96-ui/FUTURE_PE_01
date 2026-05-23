# FUTURE_PE_01 

https://claude.ai/public/artifacts/7071b84e-8cf4-4bec-ae08-cc06e75b70d0
Prompt Engineering project for generating high-converting website copy for a digital agency.
AI Website Copy Generator — Prompt Engineering Task 1 (2026)
Business Chosen

Creative websites, branding, and AI-powered content solutions for modern businesses in Vijayawada.. The business needed:

A clear value proposition 
Service descriptions that convert browsers into booked ones.
CTAs that feel local and trustworthy
A professional tone — warm but credible
Prompt Logic
Core System Design
The prompt framework is built around a Business Context Block — a reusable structured input that feeds into specialized prompts for each page section.

Every prompt follows this pattern:

ROLE → CONTEXT BLOCK → OUTPUT FORMAT → TONE CONSTRAINTS → NEGATIVE SPACE
Negative Space means explicitly telling the AI what NOT to write — e.g., "avoid clichés like 'world-class', 'passionate about', 'one-stop solution'."

Four Prompt Modules
Module	Purpose	Output
homepage.prompt.md	Hero section + intro	Headline, sub-headline, intro paragraph
services.prompt.md	Service cards	Name, description, what's included, differentiator
cta.prompt.md	Call-to-action sections	Booking CTA, trust copy, urgency/location hooks
tone-adapter.prompt.md	Tone calibration	Adjusts copy register for business type
Tool Used
Claude (Anthropic) — Primary generation tool
Model: claude-sonnet-4-20250514
Files in This Repo
/
├── README.md                         ← This file
├── prompts/
│   ├── homepage.prompt.md            ← Homepage copy prompt
│   ├── services.prompt.md            ← Services page prompt
│   ├── cta.prompt.md                 ← CTA sections prompt
│   └── tone-adapter.prompt.md        ← Tone calibration prompt
├── outputs/
│   ├── homepage-copy.md              ← Generated homepage copy
│   ├── services-copy.md              ← Generated services copy
│   └── cta-copy.md                   ← Generated CTA sections
└── generator/
    └── live-generator.jsx            ← React component with live Anthropic API
How to Reuse for Any Client
Fill in the Business Context Block in each prompt file
