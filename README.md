# Boaz Leleina — Backend & Cloud Engineer

Welcome to the repository for my personal portfolio website, built with **Astro 4**, **TailwindCSS**, and **DaisyUI**. 

This project serves as a showcase of my technical expertise, cloud engineering background, and AI integration capabilities. It is optimized for speed, responsive design, and SEO, scoring exceptionally high on core web vitals.

🔗 **Live Website**: [boazleleina.com](https://boazleleina.com) (Local dev: `http://localhost:4322`)  
🔗 **LinkedIn**: [linkedin.com/in/boaz-leleina](https://www.linkedin.com/in/boaz-leleina/)  
🔗 **X (Twitter)**: [x.com/boaz_leleina](https://x.com/boaz_leleina)  
📧 **Email**: [boazleleina3@gmail.com](mailto:boazleleina3@gmail.com)

---

## 🚀 About Me

I am a **Backend & Cloud Engineer** with production experience building resilient Python/Django, FastAPI, PostgreSQL, and AWS systems across EdTech and AI startups. 

Currently an **M.S. in Computer Science candidate** (graduating August 2026) with a perfect **4.0 GPA**, my technical focus centers on the intersection of **LLM applications**, **document-grounded assistants**, **agentic workflows**, and the **cloud architecture** that powers them.

- 🎓 **MS in Computer Science** (WJU, Rocklin, CA — GPA: 4.0)
- ☁️ **AWS Certified Cloud Practitioner**
- 🦁 **Samburu Advocate** (Keynote Speaker at *The Samburu Project* Splash Bash Gala in Los Angeles)

---

## 🛠️ Tech Stack & Engineering Practices

This portfolio was constructed to serve as a testbed for modern front-end build tools, responsive layout design, and clean web engineering:

- **Framework**: [Astro 4](https://astro.build/) — Used for island-architecture loading and ultra-fast static HTML generation.
- **Styling**: [TailwindCSS](https://tailwindcss.com/) & [DaisyUI](https://daisyui.com/) — Clean, utility-first styling utilizing high-contrast monochrome light & dark modes.
- **Package Management**: [pnpm](https://pnpm.io/) — Fast, workspace-compatible package dependency resolution.
- **SEO & Performance**: Integrated sitemap generation using `@astrojs/sitemap`, automated `robots.txt`, semantic HTML structures, and responsive image compression (`.webp` format).

---

## ⚡ Engineered Highlights of this Repository

For recruiters inspecting this codebase, here are a few custom enhancements I have engineered beyond the default template structure:

1. **State-Synchronized Dark Mode Slider**:
   - Engineered a custom, dual-control **Sun/Moon slider toggle** inside `src/components/Header.astro` (for mobile) and `src/components/SideBar.astro` (for desktop).
   - Solved Flash of Un-themed Content (FOUC) by inserting a tiny blocking script in the `<head>` of [BaseLayout.astro](src/layouts/BaseLayout.astro) to apply the localStorage theme before visual rendering begins.
   - Built state synchronization listening to Astro's `astro:after-swap` navigation lifecycle, guaranteeing theme persistence across page changes.
2. **Defensive Sitemap Integration**:
   - Debugged and patched a known sitemap generation error under certain dynamic routing environments by adding a defensive safeguard check (`_routes || []`) in the bundle structure to secure production builds.
3. **Structured Resume Web-Interface**:
   - Custom-coded a rich resume layout inside [cv.astro](src/pages/cv.astro), translating vector resume components into clean CSS components, combined with a premium top-right PDF download anchor linking directly to [Bleleina_Resume.pdf](public/Bleleina_Resume.pdf).
4. **Witty Custom 404 Experience**:
   - Customized a humorous, developer-centric [404.astro](src/pages/404.astro) page displaying my custom `avatar.webp` image, reading: *"Whoops, the cows ate my page 🐄"*—a playful Samburu-nomadic spin on the classic "dog ate my homework" joke.

---

## 📂 Key Projects Spotlighted

### 🤖 **Resume Agent** — *Python, FastAPI, Streamlit, Ollama, Qwen3, pdfplumber, Pydantic, pytest*
A privacy-preserving AI resume review tool designed to run entirely locally using Ollama.
* **Agent Architecture**: Designed an 8-stage agent pipeline with model routing across **Qwen3 4B** (for high-speed structured data extraction) and **Qwen3 8B** (for deep, reasoning-heavy resume-to-job fit analysis).
* **Parsing Engine**: Developed a robust 4-layer job description parsing engine leveraging JSON-LD metadata, BeautifulSoup, and fallback heuristic algorithms to gracefully parse inconsistent job formats.
* **Reliability & Testing**: Integrated a 25-test suite utilizing **pytest** to validate schema extraction integrity, parsing edge cases, and SSRF security boundaries.

---

## 🏗️ Local Setup & Exploration

To clone and explore this repository locally, make sure you have [Node.js](https://nodejs.org/) installed:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/boazleleina/boazleleina.com.git
   cd boazleleina.com
   ```

2. **Install Dependencies**:
   ```bash
   pnpm install
   ```

3. **Run the Local Development Server**:
   ```bash
   pnpm run dev
   ```

4. **Verify the Production Build**:
   ```bash
   pnpm run build
   ```

---

## 🤝 Let's Connect!

I am always interested in discussing document-grounded assistants, agentic pipelines, LLM fine-tuning, and robust cloud backend engineering. 

If you are a recruiter or an engineering lead looking for a cloud developer with an AI-focused mindset, feel free to review my [Resume PDF](public/Bleleina_Resume.pdf), read my CV at [/cv](https://boazleleina.com/cv), or ping me on **[LinkedIn](https://www.linkedin.com/in/boaz-leleina/)**!
