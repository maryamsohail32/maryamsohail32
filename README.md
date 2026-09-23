<!-- ============================================================
  Maryam Sohail Ahmed — GitHub profile README
  Repo: maryamsohail32/maryamsohail32
  Palette: navy #1B3A5C · amber #E8A33D
  ============================================================ -->

<div align="center">

<img src="https://raw.githubusercontent.com/maryamsohail32/maryamsohail32/main/assets/banner.svg" alt="Maryam Sohail Ahmed - Machine Learning, Karachi" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Space+Grotesk&weight=600&size=22&duration=3200&pause=1100&color=E8A33D&center=true&vCenter=true&width=680&height=40&lines=Former+ML+Intern+%40+FlyRank+AI;BS+Artificial+Intelligence+%C2%B7+DUET+Karachi;Open+to+ML+%2F+AI+internships" alt="Typing intro"/>

<br/>

<a href="https://maryamsohailahmed.vercel.app"><img src="https://img.shields.io/badge/Portfolio-1B3A5C?style=for-the-badge&logo=vercel&logoColor=E8A33D" alt="Portfolio"/></a>
<a href="https://www.linkedin.com/in/maryam-sohail-ahmed-685524341"><img src="https://img.shields.io/badge/LinkedIn-1B3A5C?style=for-the-badge&logo=linkedin&logoColor=E8A33D" alt="LinkedIn"/></a>
<a href="https://papers.ssrn.com/abstract=7453339"><img src="https://img.shields.io/badge/SSRN%20Preprint-1B3A5C?style=for-the-badge&logoColor=E8A33D" alt="SSRN preprint"/></a>
<a href="mailto:maryam786sohail@gmail.com"><img src="https://img.shields.io/badge/Email-1B3A5C?style=for-the-badge&logo=gmail&logoColor=E8A33D" alt="Email"/></a>

</div>

### 👋 Hi, I'm Maryam

I build ML systems, then I try to break my own claims before anyone else does.

I'm a 3rd-year **BS Artificial Intelligence** student at **Dawood University of Engineering & Technology (DUET), Karachi**, and a **former Machine Learning intern at FlyRank AI**. My work is applied ML for problems I can see around me: load-shedding, informal recycling, flood and heat risk, and AI literacy for students who don't get much of it.

What I care about most is the gap between *"the number looks good"* and *"the number means something."* One of my papers is literally about that.

---

## 🧭 The rule I work by

Every result in this profile carries an **evidence tag**, and every project says what it does **not** claim.

| Tag | What it means |
|---|---|
| ![Observed](https://img.shields.io/badge/OBSERVED-1B3A5C?style=flat-square) | Measured directly, on data I can name |
| ![Directional](https://img.shields.io/badge/DIRECTIONAL-E8A33D?style=flat-square) | Points a way, but the evidence is thin or unstable |
| ![Decision-support](https://img.shields.io/badge/DECISION--SUPPORT-5B7FA6?style=flat-square) | Useful for a human making a call, not for automating it |
| ![Not claimed](https://img.shields.io/badge/NOT%20CLAIMED-9AA0A6?style=flat-square) | Things I deliberately refuse to say the work proves |

---

## 🔬 Selected work

| Project | What it is | Result | Evidence | Not claimed |
|---|---|---|---|---|
| **[Chest X-Ray CNN comparison](https://github.com/maryamsohail32/ChestXRay-CNN-Temporal-Analysis)** | Three CNNs compared on the real RSNA Pneumonia Detection dataset (26,684 X-rays) | MobileNetV2: AUC **0.838**, pneumonia recall **0.85**, accuracy 0.70. The Deep CNN scored higher accuracy (0.791) but caught only **0.39** of pneumonia cases | ![Observed](https://img.shields.io/badge/OBSERVED-1B3A5C?style=flat-square) | Clinical usefulness |
| **[FlyRank content opportunity scoring](https://maryamsohail32.github.io/flyrank-ml-internship/)** | Internship capstone: end-to-end ML pipeline for ranking content refresh opportunities, deployed as a research write-up ([repo](https://github.com/maryamsohail32/flyrank-ml-internship)) | Random Forest Precision@50 = **0.76**, reversing an earlier Logistic Regression lead. Both models **underperformed the base rate** on the May holdout | ![Directional](https://img.shields.io/badge/DIRECTIONAL-E8A33D?style=flat-square) | Production-ready ranking, stability over time |
| **[KarachiWatts](https://github.com/maryamsohail32/KarachiWatts)** | Random Forest load-shedding predictor across 15 Karachi neighborhoods, with a bilingual Groq-powered chatbot on Streamlit | R² **0.991**, MAE **0.26 h** on 16,440 records | ![Observed](https://img.shields.io/badge/OBSERVED-1B3A5C?style=flat-square) on **synthetic data** | Real-world forecast accuracy |
| **[Drift Watch](https://github.com/maryamsohail32/drift-watch)** | Autonomous MLOps sentinel that detects silent ML pipeline failures and generates remediation patches. Built solo for the IBM TechXchange Dev Day Hackathon | Working submission with demo video | Not benchmarked | Detection rates on real production pipelines |
| **[SkyGuard PK](https://github.com/maryamsohail32/skyguard-pk)** | Bilingual flood and heatwave risk tool using NASA POWER satellite data and a Random Forest classifier (IBM AI Builders Challenge) | Published tool with demo | Not benchmarked | Operational early-warning use |
| **[Samajh AI](https://github.com/maryamsohail32/samajh-ai)** | Bilingual AI-literacy tutor for underserved Pakistani students. React + Vite + Tailwind on Vercel with serverless API routes | Deployed prototype | Not benchmarked | Learning-outcome impact |

<sub>Also built: [Al-Bayan](https://github.com/maryamsohail32/AlBayan) (bilingual Quranic study app, React/Flask), a [DistilBERT sentiment analyzer](https://github.com/maryamsohail32/sentiment-analyzer) (~91% on SST-2), and an interactive [Pakistan socioeconomic dashboard](https://github.com/maryamsohail32/pakistan-socioeconomic-dashboard) in Streamlit.</sub>

---

## 📄 Research

**[Accuracy is not Enough: Why Two "Good" Models Disagree on Which One is Best](https://papers.ssrn.com/abstract=7453339)** · SSRN preprint · September 2026

Which model "wins" depends on whether you rank by accuracy or by the recall of the class that matters. In pneumonia screening, those two rankings point in opposite directions.

<details>
<summary><b>🪞 Things I got wrong, and fixed</b></summary>

<br/>

- **Synthetic data, impossible metric.** My first chest X-ray model reported AUC = 1.0 on synthetic data. I noticed the result was internally inconsistent, retrained on the real RSNA dataset, and the honest numbers are above.
- **A label flaw in my FlyRank pipeline.** I caught it mid-session, corrected it, and re-ran the evaluation.
- **A model ranking that flipped.** Logistic Regression led early; Random Forest won once evaluation was done properly. I reported the reversal instead of hiding it.

Finding your own mistakes is the skill. Publishing them is the habit.

</details>

---

## 🛠️ Toolkit

Only things I have actually shipped with.

<p>
<img src="https://img.shields.io/badge/Python-1B3A5C?style=flat-square&logo=python&logoColor=E8A33D" alt="Python"/>
<img src="https://img.shields.io/badge/scikit--learn-1B3A5C?style=flat-square&logo=scikitlearn&logoColor=E8A33D" alt="scikit-learn"/>
<img src="https://img.shields.io/badge/TensorFlow-1B3A5C?style=flat-square&logo=tensorflow&logoColor=E8A33D" alt="TensorFlow"/>
<img src="https://img.shields.io/badge/Keras-1B3A5C?style=flat-square&logo=keras&logoColor=E8A33D" alt="Keras"/>
<img src="https://img.shields.io/badge/Hugging%20Face-1B3A5C?style=flat-square&logo=huggingface&logoColor=E8A33D" alt="Hugging Face"/>
<img src="https://img.shields.io/badge/pandas-1B3A5C?style=flat-square&logo=pandas&logoColor=E8A33D" alt="pandas"/>
<img src="https://img.shields.io/badge/NumPy-1B3A5C?style=flat-square&logo=numpy&logoColor=E8A33D" alt="NumPy"/>
<img src="https://img.shields.io/badge/Streamlit-1B3A5C?style=flat-square&logo=streamlit&logoColor=E8A33D" alt="Streamlit"/>
<img src="https://img.shields.io/badge/Flask-1B3A5C?style=flat-square&logo=flask&logoColor=E8A33D" alt="Flask"/>
<img src="https://img.shields.io/badge/React-1B3A5C?style=flat-square&logo=react&logoColor=E8A33D" alt="React"/>
<img src="https://img.shields.io/badge/Vite-1B3A5C?style=flat-square&logo=vite&logoColor=E8A33D" alt="Vite"/>
<img src="https://img.shields.io/badge/Tailwind-1B3A5C?style=flat-square&logo=tailwindcss&logoColor=E8A33D" alt="Tailwind"/>
<img src="https://img.shields.io/badge/Supabase-1B3A5C?style=flat-square&logo=supabase&logoColor=E8A33D" alt="Supabase"/>
<img src="https://img.shields.io/badge/Vercel-1B3A5C?style=flat-square&logo=vercel&logoColor=E8A33D" alt="Vercel"/>
<img src="https://img.shields.io/badge/SQL-1B3A5C?style=flat-square&logo=sqlite&logoColor=E8A33D" alt="SQL"/>
<img src="https://img.shields.io/badge/Git-1B3A5C?style=flat-square&logo=git&logoColor=E8A33D" alt="Git"/>
<img src="https://img.shields.io/badge/pytest-1B3A5C?style=flat-square&logo=pytest&logoColor=E8A33D" alt="pytest"/>
</p>

**LLM work:** Groq (LLaMA 3.3 70B) for chat and tutoring apps, Claude API and MCP through Anthropic Academy coursework, LangChain in competition (PROCOM'26).

---

## 🏅 Recognition

- **Top 5 scorer**, Skkillo × Sync Backend & AI Engineering Intern Challenge
- **FlyRank Machine Learning track** completed through a deployed capstone (certificate issued Sep 2026)
- **~20 Anthropic Academy certificates**, including Building with the Claude API, Model Context Protocol (intro and advanced), Agent Skills, and Subagents
- **IBM** Introduction to Artificial Intelligence (98%)
- Competitor, **LangChain Mysteries @ PROCOM'26** (FAST NUCES)

---

## 🌱 Right now

- Looking for my next **ML / AI internship**
- Entering the **Nebius × NVIDIA Global AI Hackathon**
- Preparing **Kabaad AI**, a marketplace connecting scrap sellers with verified buyers in Karachi, for the Wafi Tameer Awards RoadShow

---

## 🤝 Let's talk

Open to **ML / AI internships**, research collaborations, and projects where the honest answer matters more than the impressive one.

**[Book a look at my portfolio →](https://maryamsohailahmed.vercel.app)** · [LinkedIn](https://www.linkedin.com/in/maryam-sohail-ahmed-685524341) · [Email](mailto:maryam786sohail@gmail.com)

<img src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=120&color=1B3A5C" width="100%" alt=""/>
