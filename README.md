# Navig8.tech

<div align="center">

[![Live Demo](https://img.shields.io/badge/Demo-Live_Platform-D4AF37?style=for-the-badge&logo=googlechrome&logoColor=black)](https://rpprudenciado.github.io/Structured-Career-Roadmap-Platform-To-Support-IT-Specialization-Decisions/)
[![Bootstrap 5](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

> **Structured Career Roadmap Platform To Support IT Specialization Decisions And Job Readiness**  
> *Asia Pacific College — Bachelor of Science in Information Technology (BSIT)*

</div>

---

## Live Platform Deployment

The application is deployed live on GitHub Pages:  
**Live URL:** [https://rpprudenciado.github.io/Structured-Career-Roadmap-Platform-To-Support-IT-Specialization-Decisions/](https://rpprudenciado.github.io/Structured-Career-Roadmap-Platform-To-Support-IT-Specialization-Decisions/)

---

## Overview & Problem Context

Navig8.tech is an interactive, multi-page web platform designed to solve choice overload and decision paralysis experienced by college IT students when choosing a specialization. With thousands of scattered courses, tutorials, and certifications online, students struggle to identify what to learn first, whether a credential is free or paid, and what entry-level industry role it actually qualifies them for.

Navig8.tech organizes learning into sequenced, step-by-step pathways across 14 career specializations and 6 foundational skills. Every milestone is marked free or paid, automatically tracks progress, awards earned verification badges, and integrates a portfolio locker where students can upload, preview, and manage external credentials.

---

## Multi-Page Architecture

The platform is structured into a modular, multi-page application powered by Bootstrap 5 and client-side JavaScript state persistence:

1. **Home (`index.html`):**  
   Terminal-style hero window, floating value cards, and a dynamic 1-minute career diagnostic quiz that recommends suitable pathways based on user answers.
2. **Tracks (`tracks.html`):**  
   Catalog of 14 specializations (Cybersecurity, Cloud Computing, Networking, Software Development, Data Science, DevOps, UI/UX, etc.) and 6 foundational skills (Python, SQL, Linux, etc.) with active track selection and preview options.
3. **Roadmap (`roadmap.html`):**  
   Interactive curriculum trail featuring sequenced modules, real-time Bootstrap progress bar calculations, breadcrumbs, and automated SVG specialization badge generation upon 100% completion.
4. **Blogs (`blogs.html`):**  
   Curated library of 14 industry guidance articles and career resources organized with Bootstrap grid utilities.
5. **Profile & Portfolio (`profile.html`):**  
   Student profile dashboard with collapsible edit form, active metrics, badge locker, and external certificate management (upload, modal preview, duplicate validation, and deletion).
6. **Authentication (`auth.html`):**  
   User sign up and login with unique username validation and persistent session storage.
7. **Design System (`style.css`):**  
   Shared dark-theme CSS variables, deep back-shadow floating cards, terminal brackets, and responsive scrollbar overrides.

---

## Bootstrap 5 Component Matrix

The application implements over 10 core Bootstrap 5 components:

| Bootstrap Component | Files Implemented | Implementation Purpose |
| :--- | :--- | :--- |
| **Navbar & Hamburger** | All Pages | Sticky top navigation with mobile toggle (`.navbar-toggler`, `data-bs-toggle="collapse"`) |
| **Nav-Pills** | `index.html`, `tracks.html`, `auth.html` | Tab navigation and switching between Specializations and Skills |
| **Cards / Floating Windows** | All Pages | Deep back-shadow terminal cards with window control dots and brackets |
| **Accordion** | `index.html`, `tracks.html`, `roadmap.html`, `profile.html` | Collapsible FAQs set to closed by default with auto-retract |
| **Progress Bar** | `roadmap.html` | Dynamic real-time completion bar updated via JavaScript |
| **Breadcrumbs** | `index.html`, `tracks.html`, `roadmap.html` | Terminal-style directory path navigation |
| **Alerts** | `index.html`, `profile.html`, `auth.html` | Validation alerts and notification banners |
| **Modals** | `index.html`, `tracks.html`, `profile.html` | Dialog windows for quiz results, certificate preview, and deletion confirmation |
| **Badges & Status Pills** | All Pages | Color-coded status pills (READY, IN PROGRESS, COMPLETED) and free/paid tags |
| **Collapse** | `profile.html` | Smooth toggle container for the inline Edit Profile form |

---

## Getting Started Locally

Running Navig8.tech locally requires no build tools or package managers.

### 1. Clone the Repository
```bash
git clone https://github.com/rpprudenciado/Structured-Career-Roadmap-Platform-To-Support-IT-Specialization-Decisions.git
cd Structured-Career-Roadmap-Platform-To-Support-IT-Specialization-Decisions
```

### 2. Open in Browser
Double-click `index.html` in any modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari).

Alternatively, launch using VS Code Live Server or an HTTP server:
```bash
npx live-server .
```

---

## Academic Attribution & Integrity

- **Student Proponent:** Rhona-Mae P. Prudenciado
- **Academic Standing:** 2nd Year College Student, Bachelor of Science in Information Technology (BSIT)
- **Institution:** Asia Pacific College (APC)
- **Course:** Web Programming (WEBPROG / IT252)
- **Faculty Confidentiality:** In compliance with institutional privacy standards, faculty and instructor identities are kept strictly confidential.

---

## License

This project is licensed under the [MIT License](LICENSE).
