 some part are not vissible fr on gitbu when i lasted redme file of profile here 
https://api.github.com/repos/py43-cmd/py43-cmd/contents/assets

StatusCode: non 2xx status code (404 GET https://api.github.com/repos/py43-cmd/py43-cmd/contents/assets)
Found the issue. I checked your live profile repo and it contains only README.md — the assets/ folder was never uploaded, so these were broken:

<img src="./assets/hero.svg" ... />
<img src="./assets/footer.svg" ... />
Two stats services were also failing:

github-readme-stats.vercel.app → 503
github-readme-activity-graph.vercel.app → 402
Fixed in GITHUB_PROFILE_README.md
Replaced the local hero with an animated capsule-render gradient banner.
Replaced the local footer with an animated capsule-render gradient wave.
Switched GitHub stats and top languages to a working mirror.
Replaced the broken activity graph with working profile-summary-cards.
Kept your custom SVGs in assets/ as an optional upgrade.
All active image URLs now return HTTP 200.

What you need to do
In your py43-cmd/py43-cmd repo, replace README.md with the updated:

GITHUB_PROFILE_README.md

No extra asset upload is required now. If you later want the custom hero instead, upload assets/hero.svg and assets/footer.svg to that repo, then switch the two banner URLs back to ./assets/hero.svg and ./assets/footer.svg.

- **Highlights:** AI bug analysis, code review, API doc generation, task breakdowns, multi-turn assistant with citations

### [Skill Up](https://github.com/py43-cmd/skill_up) — Learning management system

A full-stack LMS where instructors build courses with video lectures and quizzes, students enroll and learn, and graduates earn verified certificates.

<p>
  <img src="https://img.shields.io/badge/React_19-0D0D12?style=flat-square&logo=react&logoColor=C9F75A" alt="React 19" />
  <img src="https://img.shields.io/badge/Stripe-0D0D12?style=flat-square&logo=stripe&logoColor=A78BFA" alt="Stripe" />
  <img src="https://img.shields.io/badge/Cloudinary-0D0D12?style=flat-square&logo=cloudinary&logoColor=38BDF8" alt="Cloudinary" />
  <img src="https://img.shields.io/badge/JWT-0D0D12?style=flat-square&logo=jsonwebtokens&logoColor=F4F2EC" alt="JWT" />
</p>

- **Frontend:** React 19, Vite 7, Tailwind CSS 4, shadcn/ui, React Router 7, Recharts, Zod
- **Backend:** Node.js, Express, MongoDB, JWT auth, bcrypt, rate limiting, `express-validator`
- **Integrations:** Stripe Checkout + webhooks, Cloudinary media/CDN, Nodemailer OTP email
- **Highlights:** curriculum builder, auto-graded quizzes and final exams, progress tracking, certificate downloads, instructor revenue dashboard, role-based access

### [Convertify](https://github.com/py43-cmd/convertify) — Document processing suite

A full-stack platform for converting Word ↔ PDF and merging PDFs, with session auth and secure per-request temporary storage.

<p>
  <img src="https://img.shields.io/badge/React-0D0D12?style=flat-square&logo=react&logoColor=C9F75A" alt="React" />
  <img src="https://img.shields.io/badge/Express-0D0D12?style=flat-square&logo=express&logoColor=F4F2EC" alt="Express" />
  <img src="https://img.shields.io/badge/ConvertAPI-0D0D12?style=flat-square&logoColor=A78BFA" alt="ConvertAPI" />
  <img src="https://img.shields.io/badge/pdf--lib-0D0D12?style=flat-square&logoColor=FF5F57" alt="pdf-lib" />
</p>

- **Frontend:** Vite + React, Tailwind CSS, Radix UI — glassmorphism design with micro-animations
- **Backend:** Node.js + Express, ConvertAPI, `pdf-lib`, `pdf-parse`, Multer
- **Highlights:** OCR-aware PDF → Word conversion, structural upload validation, automatic temp-file garbage collection, client-safe error handling
- **Security:** authenticated routes, extension/MIME/signature checks, encrypted-PDF rejection

---

## 📈 GitHub stats

<p align="center">
  <img
    src="https://github-readme-stats-sigma-five.vercel.app/api?username=py43-cmd&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&bg_color=0D0D12&title_color=C9F75A&text_color=F4F2EC&icon_color=A78BFA"
    alt="GitHub stats"
    width="48%"
  />
  <img
    src="https://streak-stats.demolab.com/?user=py43-cmd&hide_border=true&background=0D0D12&stroke=2A2A33&ring=C9F75A&fire=A78BFA&currStreakLabel=C9F75A&sideLabels=F4F2EC&dates=9B99A7"
    alt="GitHub streak"
    width="48%"
  />
</p>

<p align="center">
  <img
    src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=py43-cmd&layout=compact&langs_count=8&hide_border=true&bg_color=0D0D12&title_color=C9F75A&text_color=F4F2EC"
    alt="Top languages"
    width="48%"
  />
  <img
    src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=py43-cmd&theme=github_dark"
    alt="Most used languages by commit"
    width="48%"
  />
</p>

<p align="center">
  <img
    src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=py43-cmd&theme=github_dark"
    alt="GitHub profile summary"
    width="100%"
  />
</p>

---

## 🌱 Currently

- Building **DevFlow AI** — my final-year MERN + AI project
- Hardening **Convertify** and **Skill Up** for production use
- Going deeper into backend architecture, testing, RAG, and secure file handling
- Exploring UI/UX trends and web performance optimization

---

## 🤝 Let's connect

<p align="center">
  <a href="mailto:py431035@gmail.com">
    <img src="https://img.shields.io/badge/SAY_HELLO-py431035%40gmail.com-C9F75A?style=for-the-badge&labelColor=0D0D12" alt="Email Priyanshu" />
  </a>
  <a href="https://github.com/py43-cmd">
    <img src="https://img.shields.io/badge/FOLLOW-@py43--cmd-A78BFA?style=for-the-badge&labelColor=0D0D12" alt="Follow on GitHub" />
  </a>
</p>


<!-- Add these when you're ready:
<p align="center">
  <a href="https://www.linkedin.com/in/YOUR_HANDLE/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://your-portfolio.com">
    <img src="https://img.shields.io/badge/Portfolio-C9F75A?style=for-the-badge&logo=googlechrome&logoColor=0D0D12" alt="Portfolio" />
  </a>
</p>
-->

<div align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&color=0:C9F75A,55:A78BFA,100:0D0D12&height=120&section=footer&animation=twinkling"
    width="100%"
    alt="Gradient footer"
  />
</div>

<!--
  Optional: upload assets/hero.svg and assets/footer.svg to your profile repo,
  then replace the two capsule-render URLs with ./assets/hero.svg and
  ./assets/footer.svg if you want the custom animated banners instead.
-->

