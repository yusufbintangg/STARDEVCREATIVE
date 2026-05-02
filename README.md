# StarDev Creative Landing Page

> Professional web development agency landing page built with Next.js 15, React 19, and Tailwind CSS 4.

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwind-css)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript)](https://www.ecma-international.org/)
[![License](https://img.shields.io/badge/License-All_Rights_Reserved-red)](README.md)

---

## 📌 Project Overview

StarDev Creative is a modern, interactive landing page for a Indonesian web development agency. The website showcases their web development services including company profiles, e-commerce, portfolio sites, hotel booking systems, and F&B management systems. Built with performance and SEO in mind, featuring smooth animations andFully responsive design.

**Live Demo**: [https://www.stardevcreative.com](https://www.stardevcreative.com)

---

## 🛠 Tech Stack

| Category | Technology |
|----------|------------|
| **Framework** | Next.js 15.5.4 |
| **UI Library** | React 19.1.0 |
| **Styling** | Tailwind CSS 4 |
| **Animations** | Framer Motion 12, GSAP 3, Three.js |
| **Smooth Scroll** | @studio-freight/lenis |
| **Icons** | Lucide React |
| **UI Components** | Radix UI (Avatar, Dropdown, Label, Slot) |
| **Fonts** | Geist, Inter (Next.js fonts) |
| **Deployment** | Vercel |

---

## ✨ Key Features

- **Responsive Design** - Fully optimized for desktop, tablet, and mobile devices
- **Interactive Animations** - Smooth entrance animations using Framer Motion
- **Service Showcase** - Display of 6 main service categories with pricing
- **Portfolio Carousel** - Infinite bidirectional draggable portfolio gallery
- **Pricing Tables** - Comprehensive pricing packages (18 packages across 6 categories)
- **Contact Form** - Functional contact form with validation
- **WhatsApp Integration** - Direct WhatsApp contact button
- **SEO Optimized** - Complete meta tags, Open Graph, Twitter Cards,Schema.org JSON-LD
- **Smooth Scrolling** - Lenis smooth scroll implementation
- **Multi-section Layout** - Hero, Services, Pricing, About, Portfolio, Contact sections
- **Mobile Navigation** - Responsive hamburger menu with smooth scroll navigation

---

## 📁 Project Structure

```
STARDEVCREATIVE/
├── public/
│   ├── portfolio/           # Portfolio project screenshots
│   ├── project/            # Project/demo screenshots
│   └── servicepage/        # Service page images
├── src/
│   ├── app/
│   │   ├── globals.css     # Global styles
│   │   ├── layout.js       # Root layout with SEO metadata
│   │   └── page.js         # Main landing page
│   ├── components/
│   │   ├── ui/            # Reusable UI components
│   │   ├── Header.jsx      # Navigation header
│   │   ├── Footer.jsx      # Footer component
│   │   ├── HeroContent.jsx
│   │   ├── Service.jsx     # Services section
│   │   ├── PricingSection.jsx
│   │   ├── Portfolio.jsx  # Portfolio carousel
│   │   ├── ContactSection.jsx
│   │   ├── AboutUs.jsx
│   │   ├── CallToAction.jsx
│   │   ├── SupportService.jsx
│   │   ├── WorkFlow.jsx
│   │   └── WhatsAppButton.jsx
│   ├── data/
│   │   └── pricingData.js # Pricing packages data
│   └── lib/
│       └── utils.js       # Utility functions
├── components.json         # shadcn/ui components config
├── eslint.config.mjs       # ESLint configuration
├── jsconfig.json          # JavaScript config
├── next.config.mjs        # Next.js configuration
├── package.json           # Dependencies & scripts
├── postcss.config.mjs     # PostCSS configuration
└── tailwind.config.mjs   # Tailwind configuration
```

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

- **Node.js** 18.x or higher
- **npm** 9.x or higher (or yarn/pnpm/bun)

> **Note**: This project uses Next.js 15 which requires Node.js 18+

### Installation

1. **Clone the repository**
   ```bash
   cd STARDEVCREATIVE
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

### Environment Variables

This project does **not** require environment variables for local development. The contact form currently logs to console (demo mode).

| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| `ANALYZE` | Enable bundle analysis | No | `false` |

To enable bundle analyzer:
```bash
ANALYZE=true npm run build
```

---

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with Turbopack |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |

---

## 🔧 Deployment

### Deploy to Vercel (Recommended)

The easiest deployment method for Next.js applications.

**Option 1: GitHub Integration (Recommended)**

1. Push your project to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/username/stardev-creative.git
   git push -u origin main
   ```

2. Go to [Vercel Dashboard](https://vercel.com/dashboard)

3. Click "Add New Project" → "Import Git Repository"

4. Select your repository

5. Configure settings (auto-detected):
   - Framework Preset: Next.js
   - Build Command: `next build`
   - Output Directory: `.next`

6. Click "Deploy"

**Option 2: Vercel CLI**

```bash
npm install -g vercel
vercel login
vercel --prod
```

### Deployment Checklist

Before going live, verify:

- [ ] Remove all console.log statements
- [ ] Test contact form functionality
- [ ] Verify all images load correctly
- [ ] Check mobile navigation works
- [ ] Verify SEO metadata (update domain in layout.js)
- [ ] Test Lighthouse performance score
- [ ] Update Schema.org organization data

---

## 📸 Screenshots

> Add your own screenshots here

| Section | Screenshot |
|---------|-------------|
| Hero | `public/project/screencapture-inezhomestay-2025-11-22-22_43_16.png` |
| Services | `public/servicepage/` |
| Portfolio | `public/portfolio/` |

---

## 🔐 Security Notes

- The `next.config.mjs` includes security headers (X-Frame-Options, X-Content-Type-Options, Referrer-Policy, Permissions-Policy)
- Enable HTTPS in production (automatic with Vercel)
- Update the Google verification code in metadata before deploying

---

## 📄 License

All Rights Reserved. No part of this project may be reproduced or distributed without permission.

---

## 👤 Contact

**StarDev Creative** - Professional Web Development Agency

- **Website**: [https://www.stardevcreative.com](https://www.stardevcreative.com)
- **Phone**: +62 898 8025 033
- **WhatsApp**: +62 896 1686 9977
- **Email**: yusufpamungkas7@gmail.com

---

Built with ❤️ using Next.js and hosted on Vercel.
