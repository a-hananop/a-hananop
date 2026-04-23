<!-- ═══════════════════════════════════════════════════════════ -->
<!--                ABDUL HANAN SAQLAIN — README.md            -->
<!-- ═══════════════════════════════════════════════════════════ -->

<div align="center">

<!-- ── ANIMATED AVATAR ── -->
<img src="https://capsule-render.vercel.app/api?type=venom&color=0:03080f,50:061828,100:03080f&height=180&section=header&text=Abdul%20Hanan%20Saqlain&fontSize=42&fontColor=00c6ff&animation=fadeIn&fontAlignY=65&desc=AI%20Engineer%20%7C%20Builder%20%7C%20Innovator&descAlignY=85&descColor=4a9abb&descSize=16" width="100%" alt="header"/>

<br/>

<!-- ── AVATAR ORB ── -->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/a-hananop/a-hananop/main/avatar-dark.svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=1&pause=999999&color=03080f&background=03080f00&center=true&vCenter=true&width=1&height=1&lines=." alt="" width="1" height="1"/>
</picture>

<!-- Animated Ring Avatar via SVG -->
<svg width="200" height="200" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="orbGrad" cx="40%" cy="35%" r="65%">
      <stop offset="0%" stop-color="#0d2a44"/>
      <stop offset="100%" stop-color="#050f1c"/>
    </radialGradient>
    <radialGradient id="glowGrad" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#00c6ff" stop-opacity="0.15"/>
      <stop offset="100%" stop-color="#00c6ff" stop-opacity="0"/>
    </radialGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Outer glow -->
  <circle cx="100" cy="100" r="95" fill="url(#glowGrad)"/>

  <!-- Subtle rings -->
  <circle cx="100" cy="100" r="88" fill="none" stroke="#00c6ff" stroke-width="0.4" stroke-opacity="0.15"/>
  <circle cx="100" cy="100" r="76" fill="none" stroke="#00c6ff" stroke-width="0.4" stroke-opacity="0.1"/>

  <!-- Dashed orbit ring -->
  <circle cx="100" cy="100" r="88" fill="none" stroke="#00c6ff" stroke-width="1.5"
    stroke-dasharray="18 10" stroke-linecap="round" stroke-opacity="0.55">
    <animateTransform attributeName="transform" type="rotate"
      from="0 100 100" to="360 100 100" dur="8s" repeatCount="indefinite"/>
  </circle>

  <!-- Counter orbit ring -->
  <circle cx="100" cy="100" r="76" fill="none" stroke="#5060ff" stroke-width="1"
    stroke-dasharray="10 24" stroke-linecap="round" stroke-opacity="0.45">
    <animateTransform attributeName="transform" type="rotate"
      from="360 100 100" to="0 100 100" dur="12s" repeatCount="indefinite"/>
  </circle>

  <!-- Thin fast ring -->
  <circle cx="100" cy="100" r="64" fill="none" stroke="#00c6ff" stroke-width="0.7"
    stroke-dasharray="5 14" stroke-linecap="round" stroke-opacity="0.3">
    <animateTransform attributeName="transform" type="rotate"
      from="0 100 100" to="360 100 100" dur="5s" repeatCount="indefinite"/>
  </circle>

  <!-- Orbiting dot on outer ring -->
  <circle cx="188" cy="100" r="3.5" fill="#00c6ff" filter="url(#glow)">
    <animateTransform attributeName="transform" type="rotate"
      from="0 100 100" to="360 100 100" dur="8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;1;0.6" dur="8s" repeatCount="indefinite"/>
  </circle>

  <!-- Orbiting dot on middle ring -->
  <circle cx="176" cy="100" r="2.5" fill="#8060ff" filter="url(#glow)">
    <animateTransform attributeName="transform" type="rotate"
      from="180 100 100" to="-180 100 100" dur="12s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.5;0.9;0.5" dur="12s" repeatCount="indefinite"/>
  </circle>

  <!-- Orbiting dot on inner ring -->
  <circle cx="164" cy="100" r="1.8" fill="#00c6ff">
    <animateTransform attributeName="transform" type="rotate"
      from="90 100 100" to="450 100 100" dur="5s" repeatCount="indefinite"/>
  </circle>

  <!-- Core orb -->
  <circle cx="100" cy="100" r="52" fill="url(#orbGrad)" stroke="#00c6ff" stroke-width="1" stroke-opacity="0.3"/>

  <!-- Glass highlight -->
  <ellipse cx="88" cy="80" rx="18" ry="10" fill="white" fill-opacity="0.05" transform="rotate(-20 88 80)"/>

  <!-- Hex grid pattern (subtle) -->
  <g stroke="#00c6ff" stroke-width="0.4" fill="none" stroke-opacity="0.12">
    <polygon points="100,58 112,65 112,79 100,86 88,79 88,65"/>
    <polygon points="100,86 112,93 112,107 100,114 88,107 88,93"/>
    <polygon points="88,65 100,72 100,86 88,93 76,86 76,72"/>
    <polygon points="112,65 124,72 124,86 112,93 100,86 100,72"/>
  </g>

  <!-- Initials -->
  <text x="100" y="107" text-anchor="middle" fill="#00c6ff"
    font-family="'Segoe UI', Arial, sans-serif" font-size="28" font-weight="700"
    letter-spacing="3" filter="url(#glow)">AH</text>

  <!-- Pulse animation on orb -->
  <circle cx="100" cy="100" r="52" fill="none" stroke="#00c6ff" stroke-width="1.5" stroke-opacity="0">
    <animate attributeName="r" values="52;62;52" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="stroke-opacity" values="0.4;0;0.4" dur="3s" repeatCount="indefinite"/>
  </circle>

  <!-- Corner hex markers -->
  <polygon points="30,25 36,28 36,36 30,39 24,36 24,28"
    fill="none" stroke="#00c6ff" stroke-width="0.6" stroke-opacity="0.35">
    <animate attributeName="stroke-opacity" values="0.35;0.7;0.35" dur="2s" repeatCount="indefinite"/>
  </polygon>
  <polygon points="170,161 176,164 176,172 170,175 164,172 164,164"
    fill="none" stroke="#5060ff" stroke-width="0.6" stroke-opacity="0.3">
    <animate attributeName="stroke-opacity" values="0.3;0.65;0.3" dur="2.5s" repeatCount="indefinite"/>
  </polygon>
</svg>

<br/>

<!-- ── TYPING ANIMATION ── -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=18&duration=2800&pause=900&color=00C6FF&center=true&vCenter=true&width=440&lines=AI+Engineer;Generative+AI+Enthusiast;Automation+Builder;Data-Driven+Developer" alt="Typing SVG"/>

<br/>

<!-- ── STATUS BADGE ── -->
<img src="https://img.shields.io/badge/%E2%97%8F%20Available%20for%20opportunities-00e87a?style=flat-square&labelColor=030a14&color=030a14&logoColor=00e87a" alt="status"/>

<br/><br/>

<!-- ── SOCIAL BADGES ── -->
<a href="https://www.linkedin.com/in/abdul-hanan-saqlain-5a3103375/">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
&nbsp;
<a href="https://github.com/a-hananop">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>

</div>

---

## 👨‍💻 About Me

I'm an **AI Engineer** who turns ambitious ideas into working intelligent systems. I specialise in **Generative AI**, NLP pipelines, and smart automations — connecting the dots between raw data, intelligent models, and real-world applications that actually ship.

```python
class AbdulHananSaqlain:
    role       = "AI Engineer"
    focus      = ["Generative AI", "NLP", "Automation", "Full-Stack AI"]
    languages  = ["Python", "C++", "Java", "JavaScript"]
    databases  = ["MySQL", "MongoDB", "Supabase"]
    motto      = "Turning data into intelligence and ideas into reality."
```

---

## 🚀 Tech Stack

<div align="center">

### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### AI & Machine Learning
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21F?style=for-the-badge&logo=huggingface&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

### Databases
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

### Tools & Platforms
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![REST API](https://img.shields.io/badge/REST%20API-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

</div>

---

## ⚡ What I Do

<div align="center">

| | | |
|:---:|:---:|:---:|
| 🤖 **AI Applications** | 📊 **Data Analysis** | ⚙️ **Automation** |
| End-to-end AI-powered tools | Clean, model & visualise data | Smart workflow automation |
| 🌐 **Full-Stack Integration** | 🧠 **Generative AI** | 🔗 **API Integration** |
| Backend & API systems | LLM pipelines & prompting | Seamless service connections |

</div>

---

## 📊 GitHub Analytics

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=a-hananop&show_icons=true&theme=tokyonight&hide_border=true&bg_color=030a14&title_color=00c6ff&icon_color=4a9abb&text_color=6ab8d8&border_radius=12" alt="GitHub Stats"/>
&nbsp;&nbsp;
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=a-hananop&layout=compact&theme=tokyonight&hide_border=true&bg_color=030a14&title_color=00c6ff&text_color=6ab8d8&border_radius=12" alt="Top Languages"/>

<br/><br/>

<img src="https://streak-stats.demolab.com/?user=a-hananop&theme=tokyonight&hide_border=true&background=030a14&stroke=00c6ff&ring=00c6ff&fire=4a9abb&currStreakNum=eaf6ff&sideNums=6ab8d8&currStreakLabel=4a9abb&sideLabels=4a9abb&dates=1e4a62&border_radius=12" alt="GitHub Streak"/>

</div>

---

## 🏆 GitHub Trophies

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=a-hananop&theme=tokyonight&no-frame=true&no-bg=true&column=6&margin-w=6" alt="GitHub Trophies"/>

</div>

---

## 🧠 Philosophy

<div align="center">

> *"Turning data into intelligence and ideas into reality — one model at a time."*
>
> **— Abdul Hanan Saqlain**

</div>

---

## 📫 Connect With Me

<div align="center">

<a href="https://www.linkedin.com/in/abdul-hanan-saqlain-5a3103375/">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
</a>
&nbsp;
<a href="https://github.com/a-hananop">
  <img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
</a>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:03080f,50:061828,100:03080f&height=100&section=footer&fontColor=00c6ff" width="100%" alt="footer"/>

⭐ **Keep Building. Keep Learning. Keep Growing.**

</div>
