# 🥗 Ingredient Company — Landing Page
> **Online Ingredient & Meal-Kit Service | ក្រុមហ៊ុន អ៊ីនហ្គ្រីដៀន ឈុតគ្រឿងផ្សំម្ហូបស្រស់**  
> Modern, lightning-fast landing page built with **Astro**, **Tailwind CSS v4**, and a fully decoupled **JSON-driven architecture**.

[![Astro](https://img.shields.io/badge/Astro-7.x-FF5D01?logo=astro&logoColor=white)](https://astro.build/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v4.x-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Node Version](https://img.shields.io/badge/Node->=22.12.0-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![Language](https://img.shields.io/badge/Language-Khmer_%26_English-10B981)](#-bilingual-support-kmen)
[![Status](https://img.shields.io/badge/Launch-Battambang_City-047857)](#-operational-launch-zone)

---

## 📖 Overview

**Ingredient Company** (*Ingoude*) is a food-service startup revolutionizing home cooking in Cambodia. The service delivers pre-measured, recipe-ready ingredient packages (Meal Kits) directly to doorsteps, accompanied by step-by-step video tutorials and daily interactive live cooking streams.

This repository powers the official high-conversion landing page, engineered for high performance, zero unnecessary JavaScript client overhead, and instant bilingual switching.

---

## ✨ Key Features

- **⚡ Blazing Fast (Astro SSG)**: Built with Astro static-site generation for instantaneous page loads and optimal SEO.
- **🎨 Tailwind CSS v4**: Styled using the latest Tailwind CSS v4 engine for clean, modern utility-first CSS.
- **🌐 Full Bilingual Support (Khmer 🇰🇭 / English 🇬🇧)**: Instant language switcher with `localStorage` persistence and anti-flicker client execution.
- **📁 100% Decoupled JSON Architecture**: All page copy, images, dishes, pricing, and SVGs are stored cleanly inside `public/contents/`—enabling content updates without touching code.
- **🗺️ Real Interactive Battambang (BTB) Map**: Embedded Google Maps view covering priority delivery zones in Battambang City (*Svay Pao*, *Prek Preah Sdach*, *Wat Kor*, *Chamkar Samraong*).
- **📺 Ambient Live Cooking Video Background**: Seamlessly integrated, muted looping YouTube cooking show iframe with atmospheric gradient overlays.
- **🍲 Interactive Dish Explorer**: Explore authentic Cambodian dishes (*Beef Lok Lak*, *Samlor Korko*, *Lemongrass Chicken Stir-Fry*) with cook times, portion options, and ingredient lists.
- **📱 Multi-Channel Social Ordering**: Direct conversion links for Telegram bot/channel, Facebook Messenger, TikTok, and phone hotline.
- **🎯 Persona-Centric Sections**: Dedicated solution flows for university students, busy corporate professionals, and household families.

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Framework** | [Astro](https://astro.build/) (v7.x) |
| **CSS Framework** | [Tailwind CSS](https://tailwindcss.com/) (v4.x via `@tailwindcss/vite`) |
| **Icons** | [Lucide Icons](https://lucide.dev/) (`@lucide/astro`, `lucide-static`) & Optimized Inline SVGs |
| **Typography** | [Kantumruy Pro](https://fonts.google.com/specimen/Kantumruy+Pro) (Khmer) & [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) (English) |
| **Data Format** | Modular JSON schemas under `public/contents/` |
| **Runtime** | Node.js `>= 22.12.0` |

---

## 📂 Project Structure

```text
IngredientLandingPage/
├── public/
│   ├── contents/                # 📦 Data-driven content files (JSON)
│   │   ├── Benefits.json        # 6 core value benefits & SVGs
│   │   ├── Company.json         # Company metadata, navigation & social links
│   │   ├── CoreConcept.json     # Split comparison & value pillars
│   │   ├── CTASection.json      # Conversion call-to-action copy
│   │   ├── FAQ.json             # Frequently asked questions
│   │   ├── Hero.json            # Hero titles, badges, and trust stats
│   │   ├── HowItWorks.json      # 3-step ordering-to-cooking workflow
│   │   ├── LaunchZone.json      # Battambang Google Map & delivery hubs
│   │   ├── MealKits.json        # Menu catalog, ingredients, portions & pricing
│   │   ├── ProblemSolution.json # Wet market pain points vs. Ingoude solutions
│   │   ├── SocialOrdering.json  # Telegram/FB/TikTok links & YouTube video config
│   │   └── TargetAudience.json  # Personas (Students, Professionals, Families)
│   ├── audience-*.jpg           # Persona imagery
│   ├── *-dish.jpg / *.png       # High-resolution food photography
│   └── logo.png                 # Brand logo
├── src/
│   ├── components/              # 🧩 Modular Astro UI Components
│   │   ├── Benefits.astro
│   │   ├── CoreConcept.astro
│   │   ├── CTASection.astro
│   │   ├── FAQ.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── HowItWorks.astro
│   │   ├── LaunchZone.astro
│   │   ├── MealKitsExplorer.astro
│   │   ├── Navbar.astro
│   │   ├── ProblemSolution.astro
│   │   ├── SocialOrdering.astro
│   │   └── TargetAudience.astro
│   ├── layouts/
│   │   └── Layout.astro         # HTML skeleton, fonts, meta tags & language script
│   ├── pages/
│   │   └── index.astro          # Main landing page
│   └── styles/
│       └── global.css           # Global typography and Tailwind v4 configuration
├── package.json
└── astro.config.mjs
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have **Node.js 22.12.0** or later installed on your system:

```bash
node -v
```

### Installation

Clone the repository and install the project dependencies:

```bash
git clone https://github.com/your-username/IngredientLandingPage.git
cd IngredientLandingPage
npm install
```

### Running the Development Server

Start the local Astro development server:

```bash
npm run dev
```

Open your browser and navigate to [http://localhost:4321](http://localhost:4321).

#### Background Mode (Recommended for CLI / Headless)

You can run Astro dev server in the background:

```bash
npx astro dev --background
```

Manage the background process using:

```bash
npx astro dev status   # Check server status and active port
npx astro dev logs     # Stream server output
npx astro dev stop     # Stop the background process
```

---

## 📦 Production Build

To build the static production site:

```bash
npm run build
```

The compiled output will be generated inside the `./dist/` directory, ready to deploy to any static host (Cloudflare Pages, Vercel, Netlify, GitHub Pages, AWS S3, etc.).

Preview the production build locally:

```bash
npm run preview
```

---

## ⚙️ Content Management Guide (JSON Data Architecture)

All visual and textual content is separated into JSON files inside `public/contents/`. You can update content without modifying Astro templates:

| File | What You Can Edit |
|---|---|
| [`Company.json`](public/contents/Company.json) | Company name, hotline number, Telegram/FB/TikTok links, footer motto, navigation items. |
| [`MealKits.json`](public/contents/MealKits.json) | Add/modify dishes, prices, portion sizes, ingredients, difficulty, cook times, and food images. |
| [`LaunchZone.json`](public/contents/LaunchZone.json) | Battambang Google Maps embed coordinates, covered sangkats/districts, delivery hub info. |
| [`SocialOrdering.json`](public/contents/SocialOrdering.json) | Live stream schedule, YouTube background video ID (`youtubeVideoId`), ordering channel links. |
| [`Benefits.json`](public/contents/Benefits.json) | Benefit card headlines, descriptions, background photo paths, and icon SVGs. |
| [`TargetAudience.json`](public/contents/TargetAudience.json) | Target customer demographics, pain points, solutions, and background images. |
| [`FAQ.json`](public/contents/FAQ.json) | Add or edit frequently asked questions and answers in Khmer and English. |

---

## 🌐 Bilingual Support (KM/EN)

The application handles dual language support through clean CSS toggle rules:

- **Khmer elements** are wrapped with `.lang-km`.
- **English elements** are wrapped with `.lang-en`.
- When the `<html>` tag has `data-lang="km"`, `.lang-en` elements are automatically hidden via CSS, and vice versa.
- User preference is saved in `localStorage.getItem('ingoude_lang')` and loaded synchronously in `<head>` to prevent Flash of Unstyled Content (FOUC).

---

## 📄 License

This project is proprietary and developed for **Ingredient Company (Cambodia)**. All rights reserved.
