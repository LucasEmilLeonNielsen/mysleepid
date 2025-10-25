🧩 Shopify Codex Builder — Full Theme Repository

This repository contains the entire Shopify theme for your store — structured, documented, and optimized for OpenAI Codex to read, understand, and evolve.

It functions as Codex’s active memory and workspace for everything related to your storefront:
from visual sections and effects to configuration, layout logic, and customer templates.

The guiding principle remains:

Each iteration Codex produces should improve the theme without breaking its architecture.

🏗️ Structure Overview
/Shopify

This directory contains the complete live theme, directly exported from Shopify.
It mirrors the structure Shopify expects:

Shopify/
├── assets/        → JavaScript, CSS, and image assets
├── config/        → theme settings & presets
├── layout/        → layout files (e.g., theme.liquid)
├── locales/       → translations
├── sections/      → functional blocks (hero, quiz, reports, etc.)
├── snippets/      → reusable code partials
└── templates/     → page and customer templates
    └── customers/ → login, account, register templates


Purpose:

Serves as Codex’s full contextual environment for the theme.

Allows Codex to reason about the relationships between files (e.g., how layout → sections → snippets interact).

Enables precise modifications — Codex can now add new sections, extend schema, or inject logic with awareness of the entire Shopify structure.

/sections/test

This is your core custom section, manually created and vital to your product and store.

Codex must:

Preserve the integrity of this file.

Use it as a reference example of your preferred naming, structure, and style conventions.

Never overwrite or delete it without explicit instruction.

/effects

Your internal motion and visual effect library.

effectlist.txt or .md lists:

Name — effect identifier

Usage — intended application

Code — JavaScript logic

CSS — supporting styles

Codex should always check this list before creating new animations, ensuring visual consistency across all sections.

🧠 Codex Context & Goal

Codex’s task is to evolve this theme intelligently — not to reinvent it.

When generating new components, Codex must:

Use the /Shopify directory as the source of truth for theme structure.

Reference /sections/test for code style and schema patterns.

Reuse or extend effects from /effects.

Output production-ready Liquid that can be pasted or deployed directly to Shopify.

Maintain compatibility with Shopify’s Online Store 2.0 schema.

🔁 Workflow Summary

Open Codex → select this repo as the environment.

Codex reads from /Shopify to understand the full theme context.

When you prompt Codex to build or update something (e.g., “Add email capture to quiz result screen”):

It creates or modifies files inside /Shopify/sections/, /Shopify/snippets/, or /Shopify/assets/.

You review changes first (Codex does not push directly).

Once verified, you manually upload or deploy to Shopify (shopify theme push or manual import).

Commit the validated changes back to GitHub so Codex can learn from them.

🧱 Safety Rules

Codex must never edit or delete the /sections/test file unless explicitly told.

Codex must not auto-deploy — all commits require manual review.

Major structural updates should always be tested in a duplicate theme on Shopify before live deployment.

🎯 Purpose Recap

Centralize the full Shopify theme in one repository.

Give Codex total visibility into layout, schema, and logic.

Allow iterative, AI-assisted improvements — safely and reversibly.

Turn this repo into a living knowledge base for your Shopify storefront.

Author

NKK Group — TikTok-First E-Commerce
Shopify Architecture via Codex | Precision, Consistency, Scale
