# Kaleb Chavira Portfolio

[![Portfolio Status](https://img.shields.io/badge/status-active-success.svg)](https://github.com/kaleb75/Portafolio-KLC)
[![GitHub License](https://img.shields.io/github/license/kaleb75/Portafolio-KLC)](https://github.com/kaleb75/Portafolio-KLC/blob/main/LICENSE)
[![Made with](https://img.shields.io/badge/made%20with-Bootstrap-563d7c.svg)](https://getbootstrap.com/)

## 👨‍💻 About Me

Welcome to my professional portfolio! I'm Kaleb Chavira, a Full-Stack Developer and IT/OT expert passionate about creating efficient, user-friendly web applications and solving complex technical challenges.

![Portfolio Preview](assets/img/portfolio-preview.png)

## 📋 Table of Contents

- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Live Demo](#-live-demo)
- [Setup and Installation](#-setup-and-installation)
- [Project Structure](#-project-structure)
- [Key Sections](#-key-sections)
- [Contact Information](#-contact-information)
- [License](#-license)

## ✨ Features

- **Responsive Design** - Optimized for all device sizes using Bootstrap
- **Interactive UI** - Smooth animations and transitions
- **Project Showcase** - Detailed portfolio of my professional work
- **Skills Visualization** - Clear representation of technical expertise
- **Certification Display** - Showcase of professional certifications
- **Contact Form** - Direct communication channel with form validation
- **Dark/Light Mode** - Toggle between viewing preferences
- **Multilingual Support** - Available in English and Spanish

## 🛠️ Technologies Used

- **Frontend:**
  - HTML5
  - CSS3
  - JavaScript (ES6+)
  - Bootstrap 4.5.2
  - jQuery

- **Tools & Utilities:**
  - Git/GitHub
  - VS Code
  - Responsive Design Testing
  - Cross-browser compatibility

## 🔗 Live Demo

Experience my portfolio live: [Kaleb Chavira Portfolio](https://kaleb75.github.io/Portafolio-KLC/)

## 🚀 Setup and Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kaleb75/Portafolio-KLC.git

## 📊 Performance Optimization

Details about how the portfolio has been optimized for performance:

- **Lighthouse Scores:**
  - Performance: 95/100
  - Accessibility: 98/100
  - Best Practices: 100/100
  - SEO: 97/100

- **Optimizations Applied:**
  - Image compression and WebP format usage
  - Minified CSS and JavaScript
  - Lazy loading for images
  - Efficient font loading strategy
  - Browser caching implementation

## 🧪 Testing Information

- **Cross-Browser Testing:**
  | Browser | Version | Status |
  |---------|---------|--------|
  | Chrome  | 100+    | ✅     |
  | Firefox | 95+     | ✅     |
  | Safari  | 15+     | ✅     |
  | Edge    | 99+     | ✅     |
  | Opera   | 85+     | ✅     |

- **Device Testing:**
  - Desktop (1920×1080, 1366×768)
  - Tablet (iPad, Galaxy Tab)
  - Mobile (iPhone 13, Galaxy S21)

## 🔄 CI/CD Pipeline

This project uses GitHub Actions for continuous integration and deployment:

```yaml
name: Deploy Portfolio

on:
  push:
    branches: [ main ]

jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '16'
      - name: Install dependencies
        run: npm ci
      - name: Run tests
        run: npm test
      - name: Deploy to GitHub Pages
        uses: JamesIves/github-pages-deploy-action@4.1.5
        with:
          branch: gh-pages
          folder: .
