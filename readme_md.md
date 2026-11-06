# Navig8.tech 🧭
> **Designing A Structured Career Roadmap Platform To Support IT Specialization Decisions And Job Readiness**  
> *Final Project in UI/UX Design and Programming (USERDES / IT252) — Asia Pacific College*

**Navig8.tech** is an interactive, web-based career roadmap and learning path platform designed to help Information Technology (IT) and Computer Science students navigate specialization decisions with confidence. By providing structured course sequencing, cost transparency (free vs. paid), explicit job outcome linkages, and an integrated skill showcase, Navig8.tech solves the widespread issue of choice overload and disjointed learning paths.

---

## 📌 Problem Context & Market Need

In both global and local contexts, IT students face significant hurdles transitioning from classroom theory to career readiness:

- **Degree-to-Job Disconnect:** A 2025 Cengage Group study revealed that only **30%** of college graduates secured jobs related to their degree, with nearly half reporting severe job-specific skill gaps. Locally, BSIT/BSCS graduates in the Philippines score high in programming confidence but rate themselves significantly lower in certification-based and industry-aligned skills (Austria, 2025).
- **Choice Overload:** With tens of thousands of MOOCs available across fragmented platforms (YouTube, LinkedIn Learning, DataCamp, IBM SkillsBuild, Microsoft Learn), students experience decision paralysis and often abandon unsequenced learning paths (Chen et al., 2022).
- **Lack of Transparency & Job Mapping:** Learners spend time on courses without knowing upfront whether certifications require paid fees or which entry-level job roles completed modules actually qualify them for.

---

## 👤 Target User & Persona Overview

The platform was built around the specific pain points of second- and third-year IT students who have basic technical foundations but remain undecided on a career specialization.

### Persona Profile: Marco Juan Dela Torre (Age 20)
* **Program & Year:** 2nd Year BSIT Student (Metro Manila, Philippines)
* **Background:** Computer-savvy student receiving family allowance and partial scholarship. Interested in systems, networks, and security due to industry demand, but lacks clear guidance.
* **Primary Frustrations:**
  1. Overwhelmed by scattered recommendations (YouTube playlists, TikTok tips, Reddit threads).
  2. Inability to verify if a course/cert is free or paid before investing time.
  3. Completing tutorials without understanding if employers value them or what job titles they unlock.
* **Key Needs:** Cost-transparent learning paths, clear step sequencing, tangible progress tracking, and verifiable portfolio building.

---

## 🎨 UI/UX Visual System & Design Philosophy

Navig8.tech features a modern, accessible interface tailored for modern dark and light viewing environments, strictly maintaining semantic color meanings across modes.

### Color Palette & Token System

| Token Name | Hex Code / Value | Visual Role & Usage |
| :--- | :--- | :--- |
| **Shadow Grey** | Base Dark Background | High-contrast container base for Dark Mode |
| **Twilight Indigo** | Secondary Base / Accents | Structural borders, card backgrounds, and navigation elements |
| **Alabaster Grey** | Soft Light Background | Warm, non-glare background alternative to pure white for Light Mode |
| **Royal Gold** | Brand & Progress Highlight | Primary call-to-action buttons, active track indicators, key accents |
| **Emerald** | Completed / Verified Tag | Indicates completed progress steps, free tier badges, verified skills |
| **Red Ochre** | Attention / Lock Tag | Highlights locked prerequisites, paid exam alerts, switching warnings |

### Typography & Structure
- **Display & Section Titles:** `Sora`
- **Body Text & Descriptions:** `Karla` (14px – 15px)
- **Code & Technical Metadata:** `IBM Plex Mono` (Used for free/paid tags, progress metrics, step counts)

---

## 🏗️ Information Architecture & User Flow

```
1.0 Landing / Home Page (Global Header: Auth, Theme Toggle, Nav)
 ├── 2.0 Career Paths
 │    ├── 2.1 By Specialization (14 Tracks)
 │    ├── 2.2 By Skill (6 Skill-focused Tracks)
 │    └── 2.3 Interactive Quiz (Track Discovery Engine)
 ├── 3.0 Roadmap View (Progress Trail Canvas)
 │    ├── 3.1 Sequenced Course Steps & Time Estimates
 │    ├── 3.2 Curated Resource Links ([Free] / Exam Fee Notes)
 │    ├── 3.3 Job Outcome Link ([Unlocks: Entry-Level Role])
 │    └── 3.4 Track-Specific Career Articles & FAQs
 ├── 4.0 Learner Dashboard & Profile
 │    ├── 4.1 Track Metrics & Progress Bar
 │    ├── 4.2 Track Badges Gallery (Show/Hide Controls)
 │    └── 4.3 Outside Certificates Management
 └── 5.0 Career Portfolio
      ├── 5.1 Verified Skills Breakdown
      ├── 5.2 Completed Steps Portfolio
      └── 5.3 PDF Export & Downloadable Summary
```

---

## 🚀 Key Features & Implementation Details

The prototype was constructed as a fully functional client-side single-page Web Application (`HTML5`, `CSS3`, `JavaScript ES6+`).

1. **Rule-Based Track Recommendation Quiz:**  
   Helps undecided students identify suitable specializations based on their interests, background, and time commitment.
2. **Interactive Progress Trail Canvas:**  
   Visualizes track progression through explicit step statuses: **Done**, **Current**, and **Locked**. Displays real-time progress percentages and total estimated completion hours.
3. **14 Specialization & 6 Skill Tracks:**  
   Includes curated tracks across Cybersecurity, Cloud Computing, Full-Stack Web Development, Networking, Data Analytics, and more. Features single-track focus with confirmation dialogs when switching paths.
4. **Transparent Job & Cost Mapping:**  
   Every step clearly highlights if the learning resource is **FREE**, notes external certification exam fees upfront, and explicitly states the specific entry-level job role unlocked upon step completion.
5. **Dynamic Learner Profile & Shareable Portfolio:**  
   Allows users to manage external certificates, toggle badge visibility, customize personal bio details, export progress reports to **PDF**, and download verified skill summaries.
6. **Responsive UI & Accessibility:**  
   Includes Dark/Light mode toggles, terminal-style hero visual elements, mobile hamburger drawer navigation, back-to-top controls, and standard local credential management with hashed browser persistence.

---

## 🧪 User Feedback & Design Iterations

Following peer reviews and written critiques from target users, key revisions were integrated into the final build:

| Peer Feedback Point | UX Solution Implemented |
| :--- | :--- |
| *Hero and pages felt too plain/static.* | Added a terminal-style browser window container, animated "Ready" status tags, polished card elevation, and visual motif accents. |
| *Choosing multiple tracks at once was overwhelming.* | Restricted active tracking to one path at a time with a gentle confirmation modal upon switching, while listing "Related Tracks" on the roadmap. |
| *Generic course lists across different specializations.* | Replaced generic placeholders with distinct, real-world course paths and certification links tailored specifically to each track. |
| *Need for better mobile accessibility.* | Added a responsive hamburger menu drawer, responsive CSS flex/grid layouts, and a global back-to-top navigation button. |

---

## 🛠️ Project Setup & Usage

Because Navig8.tech is packaged into a self-contained web architecture, running the application locally requires no build steps or heavy dependencies.

### Running Locally

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/navig8-tech.git
   cd navig8-tech
   ```

2. **Open in Browser:**
   Simply double-click `index.html` or open it using any modern web browser (Chrome, Edge, Firefox, Safari).

   *Alternatively, launch with VS Code Live Server:*
   ```bash
   npx live-server .
   ```

---

## 🔮 Limitations & Future Roadmap

While the current version provides a complete client-side experience using local storage persistence, planned future iterations include:

- [ ] **Backend Integration:** Migration to Supabase/Firebase for secure server-side authentication and cloud database persistence.
- [ ] **AI-Assisted Career Guidance:** Implementing LLM APIs to generate dynamic, personalized project recommendations based on earned track badges.
- [ ] **Employer Live Share Links:** Generating public, cloud-hosted portfolio URLs for seamless resume integration.

---

## 📚 Key References

- **Austria, V. B. (2025).** *Assessing the IT Skills Gap: A Comparative Analysis of Tertiary IT Education in the Philippines and Industry Expectations.* ResearchGate.
- **Cengage Group. (2025).** *2025 Graduate Employability Report.* Business Wire.
- **Chen, W., et al. (2022).** *Large scale analysis of open MOOC reviews to support learners' course selection.* arXiv:2201.06967.
- **Etikan, I., Musa, S. A., & Alkassim, R. S. (2016).** *Comparison of Convenience Sampling and Purposive Sampling.* American Journal of Theoretical and Applied Statistics, 5(1), 1-4.

---

## 📝 Author & Acknowledgments

- **Proponent:** Rhona-Mae P. Prudenciado (BSIT Student, Asia Pacific College)
- **Course Instructor:** Clarice Portia Bajao
- **Submitted For:** UI/UX Design and Programming (USERDES / IT252) Finals Requirement