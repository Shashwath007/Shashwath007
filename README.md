<div align="center">

<img src="./header-banner.svg" width="100%" alt="Shashwath — AI & Data Science Engineer" />

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com/?font=Fira+Code&size=22&pause=1200&color=F5B942&center=true&vCenter=true&width=650&height=45&lines=AI+%26+Data+Science+Engineer;Published+IEEE+Access+Author;Full-Stack+%2B+ML+Builder;Turning+Signals+Into+Insight)](https://github.com/Shashwath007)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shashwathp/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shashwath007)

</div>

<br/>

## 👋 About Me

- 🎓 AI & Data Science undergraduate at **NMAM Institute of Technology** — currently in my 6th semester
- 💼 Completed a **Technology Consulting** internship at **Wipfli India LLP**, Bengaluru Delivery Center
- ✍️ Lead author of a published **IEEE Access** journal paper — see below
- 🧠 I like building the unglamorous middle layer: OCR pipelines, watermark decoders, streaming data layers — the parts that turn raw signal into something usable
- 🔭 Currently building **PromptCraft** and a **Three.js-powered portfolio** (more in [Currently Building](#-currently-building))
- 📫 Reach me on [LinkedIn](https://www.linkedin.com/in/shashwathp/)

<br/>

## 📄 Publication

![IEEE Access](https://img.shields.io/badge/IEEE_Access-Published_Author-00629B?style=for-the-badge&logo=ieee&logoColor=white)

**AURA-Net: Authorship Unification and Robustness Architecture**
A U-Net-based, dual-head (bit + presence) deep learning system for robust image watermarking that stays verifiable after **physical print-and-capture** — not just digital re-saves. Evaluated against 8 real-world attacks (JPEG compression, Gaussian blur, rescaling, low light, salt-and-pepper noise, cropping, median filtering, and print-and-capture itself).

- Personal contribution: the **decoding pipeline** — a retry-decode mechanism with Hamming-distance-based correction, presence detection, and the full robustness evaluation
- Achieved **19.84 dB PSNR**, **0.997 SSIM**, and ~0.003s inference time, with 40–44% bit accuracy retained under four combined attacks
- Originally built and presented as part of an internship selection process for a Japanese research institution

<br/>

## 🛠️ Tech Stack

<p align="left">
  <img src="https://skillicons.dev/icons?i=python,flask,react,vite,nodejs,js,html,css,git,github,docker,vscode,threejs" alt="tech stack icons" />
</p>

<br/>

## 🚀 Featured Projects

### 🎙️ VoiceDoc — Document-to-Speech Web App

[![Repo](https://img.shields.io/badge/Repo-react__TTS-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Shashwath007/react_TTS)
[![Live Demo](https://img.shields.io/badge/Live_Demo-000000?style=flat-square&logo=vercel&logoColor=white)](https://react-tts-vert.vercel.app)

Upload a photo of a printed page → OCR pulls the text out → the app reads it back to you as an MP3. Full-stack app with a Flask backend and a React/Vite frontend, built for both plain text and math-equation documents.

- OCR via **Tesseract + pytesseract**, with **OpenCV** image preprocessing ahead of it
- Text-to-speech via **gTTS**, served through a custom audio player (seek, speed, volume, MP3/TXT download)
- Full auth (salted SHA-256), SQLite-backed conversion history, light/dark mode
- Containerized with **Docker**, deployable on **Railway**; this live demo is hosted on **Vercel**
- Started life as a Flask-only MVP ([`TTS-proj`](https://github.com/Shashwath007/TTS-proj)) before being rebuilt into the full React app above

<p align="left">
  <img src="https://skillicons.dev/icons?i=flask,react,vite,python,docker" alt="voicedoc stack" />
</p>

### 📊 Superstore Data Warehouse — Medallion Architecture on Databricks

[![Repo](https://img.shields.io/badge/Repo-shashwath--dw--project-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Shashwath007/shashwath-dw-project)
[![Dashboard](https://img.shields.io/badge/Power_BI-Live_Dashboard-F2C811?style=flat-square&logo=powerbi&logoColor=black)](https://app.powerbi.com/links/eXs8qx-Xeq?ctid=51697115-1ecd-42b5-b509-2d62c3919f76&pbi_source=linkShare)

An end-to-end data warehouse built during a data engineering internship: **Bronze → Silver → Gold** on Databricks, feeding a 7-page Power BI dashboard — extended with a real-time streaming pipeline and an ML forecasting layer.

- **Batch:** 9,994-row Kaggle Superstore dataset cleaned into a star schema (1 fact + 4 dimension tables, 10K+ fact rows) using PySpark + Delta Lake
- **Streaming:** a fake order generator every 5s → Silver cleaning → Gold aggregation every 20s → a live Power BI page over DirectQuery
- **ML:** Spark MLlib Linear Regression forecasting sales, profit, and orders 3 months out (R² up to 0.69 overall)
- **Validated:** a dedicated data-quality test suite (5/5 checks passing) catching null keys, bad dates, and negative sales before they hit Silver

<p align="left">
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white" alt="Databricks"/>
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" alt="PySpark"/>
  <img src="https://img.shields.io/badge/Delta_Lake-00ADD8?style=flat-square" alt="Delta Lake"/>
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI"/>
</p>

<details>
<summary><b>📌 At a glance (live, auto-updating)</b></summary>
<br/>

<table>
<tr>
<td><img src="https://github-stats-extended.vercel.app/api/pin/?username=Shashwath007&repo=react_TTS&theme=tokyonight&hide_border=true" alt="react_TTS repo card"/></td>
<td><img src="https://github-stats-extended.vercel.app/api/pin/?username=Shashwath007&repo=shashwath-dw-project&theme=tokyonight&hide_border=true" alt="shashwath-dw-project repo card"/></td>
</tr>
</table>

</details>

<br/>

## 🔭 Currently Building

- **PromptCraft** — a single-file prompt-engineering tool with 9 LLM providers (Anthropic, OpenAI, Gemini, Groq, Mistral, DeepSeek, and more), turning rough context into a polished, structured prompt through guided clarifying questions
- **Developer Portfolio** — a single-page site with a Three.js particle background, GSAP ScrollTrigger animations, and a dual-ring magnetic cursor
- **CALFV** — comparing TCN/Transformer architectures against LightGBM and SVR for electrochemistry sensor data (carbon + iron vanadate composite electrodes), with SHAP interpretability

<br/>

## 📊 GitHub Overview

<table>
<tr>
<td><img src="./profile/stats.svg" alt="GitHub stats"/></td>
<td><img src="./profile/top-langs.svg" alt="Top languages"/></td>
</tr>
</table>

<img src="./profile/streak.svg" alt="GitHub streak stats" width="100%"/>

<sub>⚙️ These three are self-generated by <code>readme-stats.yml</code> using a personal token, so they include private repo/contribution data — not the public Vercel endpoint, which can only see what's public.</sub>

<br/>

## 🐍 Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Shashwath007/Shashwath007/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Shashwath007/Shashwath007/output/github-contribution-grid-snake.svg" />
  <img alt="a snake eating my GitHub contribution graph" src="https://raw.githubusercontent.com/Shashwath007/Shashwath007/output/github-contribution-grid-snake.svg" width="100%"/>
</picture>

<sub>⚙️ Powered by the <code>snake.yml</code> workflow below — see setup notes. The same workflow also outputs a <a href="https://raw.githubusercontent.com/Shashwath007/Shashwath007/output/github-contribution-grid-snake.gif">GIF version</a> for places that don't render animated SVGs (LinkedIn, resume, portfolio).</sub>

<br/>
<br/>

<div align="center">

### 📫 Let's connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shashwathp/)
[![GitHub](https://img.shields.io/badge/Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Shashwath007)

<sub>Thanks for stopping by ⭐</sub>

</div>
