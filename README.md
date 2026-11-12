<p align="center">
  <img src="https://raw.githubusercontent.com/avipednekar/avipednekar/main/assets/profile-banner.svg" width="100%" alt="Avinash Pednekar — Software Developer | Cloud &amp; Applied AI" />
</p>

<div align="center">
  <h1>Hi, I'm Avinash 👋</h1>
  <p><strong>Backend &amp; Full-Stack Engineering · Cloud Infrastructure · Applied AI</strong></p>
  <p>
    <a href="https://linkedin.com/in/avinash-pednekar"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
    <a href="mailto:avinashpednekar431@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
    <a href="https://leetcode.com/u/Avinashp2004"><img src="https://img.shields.io/badge/LeetCode-D97706?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
    <a href="https://github.com/avipednekar"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
    <a href="https://instagram.com/avinashpednekar_"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" /></a>
  </p>
  <p><img src="https://img.shields.io/badge/Open%20to%20Internships%20%26%20Entry%2DLevel%20Roles-15803D?style=for-the-badge" alt="Open to Internships &amp; Entry-Level Roles" /></p>
  <p><a href="#-about-me">About</a> · <a href="#-featured-projects">Projects</a> · <a href="#-technical-skills">Skills</a> · <a href="#-github-activity--problem-solving">Activity</a> · <a href="#-lets-connect">Contact</a></p>
</div>

---

## 👨‍💻 About Me

Final-year B.Tech Computer Science and Engineering student at **KIT's College of Engineering, Kolhapur**. I build applications that connect backend APIs, databases, cloud infrastructure, and machine learning—from an AWS uptime monitor to an AI recruitment platform and a multimodal deepfake research studio.

**Open to software development internships and entry-level roles**, with a focus on Java/Spring Boot, Python, and full-stack development.

🎓 **Class of 2027** · **CGPA 8.4** · 📍 **Maharashtra, India**

---

## 🚀 Featured Projects

### ☁️ [PulseCheck — Cloud Uptime Monitoring Platform](https://github.com/avipednekar/Pulse-Check)

<p><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Flask-111827?style=flat-square&logo=flask&logoColor=white" alt="Flask" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/AWS-D97706?style=flat-square" alt="AWS" />
<img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" /></p>

An end-to-end monitoring project covering application development, infrastructure provisioning, automated delivery, and operational alerts.

- Built scheduled availability and latency checks every **10 minutes**, rolling **24-hour uptime** calculations, REST APIs, and a Chart.js dashboard.
- Provisioned a VPC, public/private subnets, EC2, private RDS PostgreSQL, ECR, and IAM roles using **Terraform**.
- Automated linting, pytest checks, container builds, and EC2 deployment through **GitHub Actions**, with temporary SSH access revoked by a cleanup step.
- Added **CloudWatch and SNS alerts** for CPU utilization and instance health; packaged the application in a non-root Docker image served by Gunicorn.

---

### 🔍 [Multimodal Deepfake Detection Studio](https://github.com/Abhijeet12N/Multimodal-deepfake)

<p><img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
<img src="https://img.shields.io/badge/Flask-111827?style=flat-square&logo=flask&logoColor=white" alt="Flask" />
<img src="https://img.shields.io/badge/Xception-6366F1?style=flat-square" alt="Xception" />
<img src="https://img.shields.io/badge/Wav2Vec%202.0-0891B2?style=flat-square" alt="Wav2Vec 2.0" />
<img src="https://img.shields.io/badge/AASIST-7C3AED?style=flat-square" alt="AASIST" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV" /></p>

A research application for examining visual manipulation and synthetic speech through multimodal inference and interactive audio diagnostics.

- Combined **Xception facial features**, **Wav2Vec 2.0 speech embeddings**, and a **3D/2D CNN audiovisual compatibility stream** through late fusion, with task-specific video, audio, and overall prediction heads.
- Built a standalone audio scanner with interchangeable **Wav2Vec, AASIST, and AASIST-L** adapters; integrated a fine-tuned AASIST checkpoint selected using validation results.
- Developed a Flask interface with model selection, overlapping-window analysis, timestamped diagnostics, recording scores and thresholds, and linked segment playback.
- Improved preprocessing consistency, preserved model-specific score directions, and added checkpoint/provenance checks and reproducible evaluation reports.

**Recorded benchmark:** **99.69% overall accuracy** and **0.9994 ROC AUC** on a saved FakeAVCeleb test set of **3,276 examples**. These are historical benchmark measurements; the Studio remains a research prototype, with audio generalization and calibration still in progress.

<details>
<summary><strong>Evaluation context and current engineering focus</strong></summary>

- The multimodal benchmark is class-imbalanced; overall balanced accuracy is approximately **99.19%**.
- The selected fine-tuned AASIST checkpoint recorded **0.999649 validation ROC AUC** on **10,511 recordings**. Validation performance is separate from held-out deployment performance.
- In an exploratory check of eight reserved, provisionally labeled audio clips, the selected model correctly classified **3/8** and incorrectly flagged all four provisionally genuine clips. This small check exposes transfer limitations; it is not a general accuracy estimate.
- Current priorities are independent recording-level calibration, final held-out audio evaluation, more representative test data, and improved audiovisual alignment.
- The November 2026 project report records **24 Python regression tests** passing for the fine-tuned integration and **17 earlier JavaScript regression tests** for result presentation. These validate software behavior, not detection accuracy.

The project integrates upstream Xception, Wav2Vec 2.0, and AASIST architectures; its contributions center on the application pipeline, model adapters, diagnostics, and evaluation workflow.

</details>

---

### 💼 [AI Recruitment Platform](https://github.com/avipednekar/Job-Recruitment)

<p><img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React" />
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
<img src="https://img.shields.io/badge/Express-111827?style=flat-square&logo=express&logoColor=white" alt="Express" />
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
<img src="https://img.shields.io/badge/Flask-111827?style=flat-square&logo=flask&logoColor=white" alt="Flask" />
<img src="https://img.shields.io/badge/Sentence%20Transformers-6366F1?style=flat-square" alt="Sentence Transformers" />
<img src="https://img.shields.io/badge/Gemini%20API-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini API" /></p>

A recruitment application connecting candidate profiles and resumes with relevant job opportunities.

- Built a **three-service architecture**: React frontend, Node.js/Express API, and a Python/Flask AI service.
- Integrated resume parsing, semantic candidate-job matching, personalized job ranking, and Gemini-powered resume-to-job-description scoring and skill-gap recommendations.
- Implemented **JWT authentication, email-OTP verification, and role-based access** for candidate and recruiter workflows.
- Added application tracking, saved jobs, and recommendation fallbacks when the AI service is unavailable.

---

### 🏦 [Online Banking System](https://github.com/avipednekar/Online-Banking-System)

<p><img src="https://img.shields.io/badge/Java-E76F00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
<img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security" />
<img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
<img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway" /></p>

An educational banking application focused on authentication, transaction integrity, and customer/admin workflows.

- Implemented account management, KYC review, beneficiary verification, transaction history, and approval workflows for higher-value transfers.
- Used **idempotency keys and ordered pessimistic balance locks** to support safe transfer retries and concurrent account updates, with debit/credit ledger records.
- Added JWT access tokens, rotating refresh tokens, **Argon2id password hashing**, role-based authorization, and Flyway-managed schema migrations.

**More work:** [Training & Placement System](https://github.com/avipednekar/Training-Placement) — student, company, and admin workflows with eligibility-based shortlisting and skill matching.

---

## 🛠️ Technical Skills

<table>
  <tr>
    <td><strong>Languages</strong></td>
    <td><img src="https://img.shields.io/badge/Java-E76F00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
      <img src="https://img.shields.io/badge/JavaScript-B8860B?style=flat-square&logo=javascript&logoColor=white" alt="JavaScript" />
      <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white" alt="C++" /></td>
  </tr>
  <tr>
    <td><strong>Backend &amp; APIs</strong></td>
    <td><img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
      <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security" />
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
      <img src="https://img.shields.io/badge/Express.js-111827?style=flat-square&logo=express&logoColor=white" alt="Express.js" />
      <img src="https://img.shields.io/badge/Flask-111827?style=flat-square&logo=flask&logoColor=white" alt="Flask" /><br />REST APIs · JWT · Role-based access control</td>
  </tr>
  <tr>
    <td><strong>Frontend</strong></td>
    <td><img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React" />
      <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5" />
      <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css&logoColor=white" alt="CSS3" />
      <img src="https://img.shields.io/badge/Tailwind%20CSS-0891B2?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
      <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" /></td>
  </tr>
  <tr>
    <td><strong>Databases</strong></td>
    <td><img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
      <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB" />
      <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway" /></td>
  </tr>
  <tr>
    <td><strong>Cloud &amp; DevOps</strong></td>
    <td><img src="https://img.shields.io/badge/AWS-D97706?style=flat-square" alt="AWS" />
      <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
      <img src="https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker Compose" />
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" /><br />EC2 · VPC · RDS · ECR · IAM · CloudWatch · SNS</td>
  </tr>
  <tr>
    <td><strong>AI &amp; ML</strong></td>
    <td><img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch" />
      <img src="https://img.shields.io/badge/Hugging%20Face-A16207?style=flat-square&logo=huggingface&logoColor=white" alt="Hugging Face" />
      <img src="https://img.shields.io/badge/scikit%2Dlearn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn" />
      <img src="https://img.shields.io/badge/Gemini%20API-4285F4?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini API" /><br />CNNs · Wav2Vec 2.0 · AASIST integration · Sentence Transformers</td>
  </tr>
  <tr>
    <td><strong>Testing &amp; Tools</strong></td>
    <td><img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="pytest" />
      <img src="https://img.shields.io/badge/JUnit-25A162?style=flat-square&logo=junit5&logoColor=white" alt="JUnit" />
      <img src="https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white" alt="Jest" />
      <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white" alt="Postman" />
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
      <img src="https://img.shields.io/badge/Linux-111827?style=flat-square&logo=linux&logoColor=white" alt="Linux" /><br />MockMvc · VS Code · Google Colab · Jupyter Notebook</td>
  </tr>
  <tr>
    <td><strong>CS Fundamentals</strong></td>
    <td>Data Structures &amp; Algorithms · OOP · DBMS · Operating Systems · Computer Networks · SDLC</td>
  </tr>
</table>

## 🎓 Education & Certifications

**B.Tech in Computer Science and Engineering**  
KIT's College of Engineering, Kolhapur · **2023–2027 (expected)** · **CGPA: 8.4**

- ☁️ **AWS Academy Graduate — Cloud Architecting** · September 2026
- 🛡️ **Google Cloud Cybersecurity — Google** · February 2026
- 🤖 **Getting Started with AI — IBM** · July 2026

---

## 📊 GitHub Activity & Problem Solving

<div align="center">
  <a href="https://github.com/avipednekar">
    <img src="https://github-readme-stats-fast.vercel.app/api?username=avipednekar&show_icons=true&theme=tokyonight&hide_border=true&border_radius=12" alt="Avinash's GitHub activity statistics" width="49%" />
  </a>
  <a href="https://github.com/avipednekar?tab=repositories">
    <img src="https://github-readme-stats-fast.vercel.app/api/top-langs/?username=avipednekar&layout=compact&theme=tokyonight&hide_border=true&border_radius=12" alt="Languages in Avinash's GitHub repositories" width="49%" />
  </a>
  <br /><br />
  <a href="https://github.com/avipednekar">
    <img src="https://streak-stats.demolab.com/?user=avipednekar&theme=tokyonight&hide_border=true&border_radius=12" alt="Avinash's GitHub contribution streak" width="75%" />
  </a>
  <br /><br />
  <a href="https://leetcode.com/u/Avinashp2004">
    <img src="https://leetcard.jacoblin.cool/Avinashp2004?theme=dark&font=Fira%20Code" alt="Avinash's LeetCode problem-solving statistics" width="65%" />
  </a>
</div>

---

## 🤝 Let's Connect

Interested in discussing an internship, an entry-level software role, or one of these projects?  
**[Email me](mailto:avinashpednekar431@gmail.com)** or **[connect on LinkedIn](https://linkedin.com/in/avinash-pednekar)**.

<div align="center">
  <br />
  <img src="https://komarev.com/ghpvc/?username=avipednekar&color=1D4ED8&style=flat-square&label=PROFILE+VIEWS" alt="GitHub profile views" />
</div>
