<p align="center">
<picture>
  <source media="(max-width: 767px)" srcset="assets/hero-narrow.svg"/>
  <img width="100%" src="assets/hero.svg" alt="Thamer Khaskhoussi. Full-Stack Developer, becoming a Software Engineer. ERP and clinic software used by 20+ businesses and 10+ clinics. Sfax, Tunisia, UTC+1, remote. Stack: TypeScript, React, Node.js, Python. Open to remote software engineering roles."/>
</picture>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/thamer-k/"><img height="52" src="assets/btn-linkedin.svg" alt="LinkedIn: in/thamer-k"/></a>&nbsp;
  <a href="mailto:tkhaskhoussi@gmail.com"><img height="52" src="assets/btn-email.svg" alt="Email: tkhaskhoussi@gmail.com"/></a>&nbsp;
  <a href="https://www.freelancer.com/u/Ugranda"><img height="52" src="assets/btn-freelancer.svg" alt="Freelancer: 5 stars, u/Ugranda"/></a>
</p>

## `~$ ls ~/shipped`

<p align="center">
<picture>
  <source media="(max-width: 767px)" srcset="assets/impact-narrow.svg"/>
  <img width="100%" src="assets/impact.svg" alt="In production. SPID Pro: multi-tenant ERP (invoicing, inventory, HR, payroll, treasury, reporting) used by 20+ businesses. SPID Med: medical practice management (Electron, real-time, encrypted patient data) in 10+ clinics. SPID Car: fleet rental platform with real-time GPS tracking, 5 operators at launch. Khloé Collection: offline-first POS and e-commerce for a fashion boutique (PWA/Electron, IndexedDB sync), delivered 2025."/>
</picture>
</p>

*These live in private client repositories. I'm happy to walk through the architecture and code on a call.*

## `~$ whoami`

I'm a full-stack developer at **[SPID Technologie](https://spid-tech.com.tn)**, where I design, build, deploy and maintain business apps end to end. I'm on track to become a **software engineer** once I finish my degree.

In the evenings I'm studying for a software engineering degree at **IIT** (expected 2027), on top of a **B.Sc. in Big Data & Data Analysis**. I speak Arabic, French and English.

## `~$ cat ship.log`

<p align="center">
<picture>
  <source media="(max-width: 767px)" srcset="assets/ship-log-narrow.svg"/>
  <img width="100%" src="assets/ship-log.svg" alt="Delivery, end to end, schema to server, as a deploy log. schema: data model (PostgreSQL, SQL Server). api: REST and real-time (Express, Zod, JWT, Socket.io). ui: web, desktop, offline (React, Electron, PWA). ci: tests and builds (GitHub Actions, Vitest, Playwright). deploy: containers on a VPS (Docker, Nginx). live: running in production."/>
</picture>
</p>

## `~$ ls ~/public`

### HELM · end-to-end BI platform &nbsp;[![th23mer/helm-bi-platform](https://img.shields.io/badge/th23mer%2Fhelm--bi--platform-2A2019?style=flat-square&logo=github&logoColor=F5A524)](https://github.com/th23mer/helm-bi-platform)

An academic capstone built on **WideWorldImporters**, taking raw OLTP rows all the way to a local AI analyst. It runs fully on-prem with no cloud APIs, and the assistant answers from real cube query results instead of guessing.

```mermaid
flowchart LR
    SRC[("WideWorldImporters<br/>OLTP")] -->|SSIS incremental ETL| DW[("SQL Server DW<br/>galaxy schema")]
    DW --> CUBE{{"SSAS cube<br/>6 dims · 9 measure groups · 4 KPIs"}}
    DW --> ML["Python ML<br/>forecast · OTIF · reorder"]
    ML -->|ML write-back| DW
    CUBE --> API["FastAPI<br/>SQL · MDX · LLM endpoints<br/>TTL caching"]
    DW --> API
    API --> UI["React + Vite + TS<br/>Operations · OLAP Analytics"]
    API <-->|cube query results| LLM["Ollama<br/>local LLM assistant"]

    classDef store fill:#1D1712,stroke:#F5A524,color:#F4EDE4;
    classDef compute fill:#1D1712,stroke:#FF7A59,color:#F4EDE4;
    classDef ui fill:#1D1712,stroke:#8FD18B,color:#F4EDE4;
    class SRC,DW,CUBE store;
    class ML,API compute;
    class UI,LLM ui;
```

<p align="center">
  <img width="80%" src="assets/helm-assistant.png" alt="HELM's local LLM assistant answering &quot;Which products are below reorder point and what should I order?&quot; with a table built from cube and ML results"/>
</p>

### JobLinker · full-stack job board &nbsp;[![th23mer/joblinker](https://img.shields.io/badge/th23mer%2Fjoblinker-2A2019?style=flat-square&logo=github&logoColor=F5A524)](https://github.com/th23mer/joblinker)

A job board with separate spaces for **candidates, recruiters and admins**. MIT licensed.

- **Frontend:** React 19, TypeScript, Vite, Tailwind v4, shadcn/ui, React Router 7
- **Backend:** Express 5 + TypeScript, JWT role-based access control, bcrypt, Multer, Nodemailer
- **Data:** PostgreSQL with raw SQL and no ORM, in a layered architecture with dependency inversion
- **Quality:** bilingual FR / EN UI, and **Lighthouse accessibility ≥ 90 enforced in GitHub Actions**

<p align="center">
  <img width="440" src="assets/joblinker-layers.svg" alt="JobLinker layers: Routes, Controllers, Services, Repositories, PostgreSQL. Each layer depends on interfaces, not on the concrete layer below. CI gate: Lighthouse accessibility 90 or above."/>
</p>

## `~$ which --all`

<p align="center">
<picture>
  <source media="(max-width: 767px)" srcset="assets/stack-narrow.svg"/>
  <img width="100%" src="assets/stack.svg" alt="Toolbox. Languages: TypeScript, JavaScript, Python. Frontend: React, Next.js, Redux, Zustand, Tailwind. Backend: Node.js, Express, FastAPI, Zod, JWT, Socket.io, Sequelize. Data and AI: PostgreSQL, SQL Server, SSIS/SSAS, pandas, NumPy, Ollama. Delivery: Docker, Nginx, GitHub Actions, VPS. Apps: Electron, PWA, IndexedDB. Testing: Vitest, Jest, Playwright."/>
</picture>
</p>

## `~$ git log --graph`

<p align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="profile-3d-contrib/profile-night-green.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="profile-3d-contrib/profile-green-animate.svg"/>
  <img width="100%" src="profile-3d-contrib/profile-green-animate.svg" alt="3D contribution graph of th23mer"/>
</picture>
</p>

## `~$ logout`

Have a product to ship, or a system to keep running? Reach me on **[LinkedIn](https://www.linkedin.com/in/thamer-k/)** or at **[tkhaskhoussi@gmail.com](mailto:tkhaskhoussi@gmail.com)**.

<p align="center">
<picture>
  <source media="(max-width: 767px)" srcset="assets/footer-narrow.svg"/>
  <img width="100%" src="assets/footer.svg" alt="Connection to github.com/th23mer closed. Thanks for reading."/>
</picture>
</p>
