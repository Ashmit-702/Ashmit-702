<div align="center">
  <img src="./assets/header.svg" alt="Ashmit Singh. B.Tech Computer Engineering, 2023–2027" width="100%"/>
</div>

<br/>

<div align="center">
  <img src="./assets/currently.svg" alt="Currently interning at Cerebro Tech." width="100%"/>
</div>

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## Special Mention

<div align="center">
  <a href="https://gitwicket-ten.vercel.app">
    <img src="./assets/gitwicket.svg" alt="GitWicket: GitHub and LeetCode activity mapped to a six-stat cricket player card" width="100%"/>
  </a>
</div>

<br/>

**GitWicket** turns public GitHub and LeetCode activity into a cricket player card. Commits become strike rate, pull requests become wickets, stars become boundaries. It then goes a step further with a **Career Card** that combines GitHub, CV, LeetCode and career goals into an evidence-based profile: what your public work supports, what is missing, and what to do next.

- Card images are rendered per request as PNGs with `@vercel/og`, so they can be embedded anywhere an image can
- Six signals are pulled from the GitHub GraphQL API and mapped to cricket stats by a rating engine; LeetCode cards use solved counts, acceptance rate and contest history, with tiers gated so volume alone can't reach the top
- Results are cached in Redis for six hours to stay inside API limits
- Includes a Compare view for putting two profiles side by side

<sub>Next.js · TypeScript · Tailwind CSS · GitHub GraphQL · Redis · Vercel</sub><br/>
[GitHub](https://github.com/Ashmit-702/Gitwicket) · [Live](https://gitwicket-ten.vercel.app)

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## Flagship Projects

<table>
<tr>
<td width="50%" valign="top">

### Dadi Ki Dawai
*A multilingual AI health companion with an Indian grandmother's voice.*

Symptom chat, urgency triage, drug guides, lab-report interpretation and first aid in one installable app.

- Replies in the language of the latest message: Hindi, Hinglish or English
- Triage returns structured JSON: urgency score, likely conditions, red flags
- Lab values extracted from PDFs and photos (PyMuPDF, Groq vision)
- Rotates Groq API keys on rate limits; ships as an installable PWA

<sub>Flask · Groq · PyMuPDF · PWA · Render</sub><br/>
[GitHub](https://github.com/Ashmit-702/final-health) · [Live](https://dadi-healthchat.onrender.com/)

</td>
<td width="50%" valign="top">

### Mainland
*A Mahabharata-inspired arcade dungeon crawler.*

You play Arjun, descending seven floors toward the Field of Kurukshetra to recover the Brahmastra.

- Python serverless functions on Vercel generate each floor procedurally (BSP), with allies introduced in a fixed story order
- Gemini writes NPC dialogue, boss taunts and floor narration; every line has a scripted fallback
- Frontend is vanilla JavaScript on a 2D canvas, no framework

<sub>Python · Vercel Serverless · Gemini API · Vanilla JS · Canvas</sub><br/>
[GitHub](https://github.com/Ashmit-702/Mainland) · [Play](https://mainland-iota.vercel.app)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### NetaBoard
*Politics, with receipts.*

An editorial political product built around evidence rather than opinion: what was said, what changed, and what the record shows.

- Claims → evidence → verdicts ledger for politicians, alongside elections and a daily brief
- Ingests live news (GDELT plus optional news APIs), then clusters and ranks it into current affairs
- Shows honest empty states instead of fabricated data when a source is missing
- Versioned SQL migrations on Supabase, Vercel Cron for refreshes, unit tests for the news and ranking engine

<sub>Next.js 14 · Supabase · PostgreSQL · Vercel Cron</sub><br/>
[GitHub](https://github.com/Ashmit-702/Netaboard) · [Live](https://neta-ashen.vercel.app)

</td>
<td width="50%" valign="top">

### SentiFi
*Market chatter, turned into BUY / HOLD / SELL signals.*

A sentiment pipeline and dashboard for stock tickers, with a REST API over the results.

- VADER sentiment with a finance-specific lexicon, run over Indian financial news (RSS, Google News) and tweets via Tweepy
- NumPy signal engine: weighted scoring, normalisation and thresholds
- FastAPI endpoints for analysis, signals, price data and history
- Plotly Dash dashboard with yfinance prices; signal history stored in PostgreSQL

<sub>FastAPI · Pandas · NumPy · Plotly Dash · PostgreSQL · Render</sub><br/>
[GitHub](https://github.com/Ashmit-702/Stockfi) · [Live](https://stockfi-uq2v.onrender.com/dashboard/)

</td>
</tr>
</table>

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## More Projects

| Project | What it does | Stack | Links |
|:--|:--|:--|:--|
| **ASHLYSIS** | Mines past exam papers for recurring questions and topics, then builds a preparation strategy. Extracts text with pdfplumber and PyMuPDF (vision fallback for scans), clusters questions with a hand-written TF-IDF and cosine similarity, and uses Groq for structured extraction and study guidance. | Flask · Groq · pdfplumber · PyMuPDF | [GitHub](https://github.com/Ashmit-702/Ashlysis-done) · [Live](https://ashlysis.onrender.com) |
| **DOSSIER** (CV Analyze) | Explainable résumé-to-job matching. Scores across five independently weighted dimensions and gives a reason for every number, with semantic matching, a what-if skill simulator and batch comparison. | FastAPI · sentence-transformers · Docker Compose | [GitHub](https://github.com/Ashmit-702/CV-Analyze) · [Live](https://cv-analyze-liard.vercel.app) |
| **One** | Constraint-based product recommender that returns a single pick with a one-line reason. Web retrieval, local LLM extraction and generic weighted scoring. | FastAPI · Ollama · SQLite | [GitHub](https://github.com/Ashmit-702/One) |
| **SecurePass Toolkit** | Password generator, breach checker and encrypted vault that run entirely in the browser: Web Crypto (AES-256-GCM, PBKDF2) and HIBP k-anonymity. | Next.js · Web Crypto | [GitHub](https://github.com/Ashmit-702/Passwrod-O) |
| **Vitals+** | A BMI calculator grown into a health-analytics app with trend charts, forecasting and AI insights that fall back to rules when the API is rate-limited. | Python · Flask · Gemini | [GitHub](https://github.com/Ashmit-702/OIBSIP-f) |
| **Station** | Weather app designed as a physical instrument panel. The API key stays server-side. | Flask · Vanilla JS · pytest | [GitHub](https://github.com/Ashmit-702/Station-Weather) |

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## Other Builds

| Project | Description | Stack | Repository |
|:--|:--|:--|:--|
| **LinkedIn CRM** | LinkedIn API research and CRM work from my internship. | LinkedIn API | [GitHub](https://github.com/Ashmit-702/Linnkedin-CRM) |
| **Autonomous AI Creator** | A self-running publishing persona. Discovers topics from Hacker News, arXiv and GitHub; an LLM editor picks at most one and logs why it rejected the rest; Redis remembers what it has already covered. | TypeScript · Next.js · Redis | [GitHub](https://github.com/Ashmit-702/Autonomous-ai-creator) |
| **URL Shortener** | Short links with click analytics (device, browser, OS, referrer). IP addresses are stored only as SHA-256 hashes. | Node.js · Express · PostgreSQL | [GitHub](https://github.com/Ashmit-702/Urlshortener) |

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## How I Ship

<div align="center">
  <img src="./assets/pipeline.svg" alt="Workflow: research, design, build, integrate, verify, ship" width="100%"/>
</div>

<br/>

The stages are the same across projects; what changes is the stack. A few patterns you can find in the repositories above:

| Pattern | Where it shows up |
|:--|:--|
| Graceful degradation for LLM calls | Dadi (API key rotation), Mainland (scripted fallbacks), Vitals+ and ASHLYSIS (rule-based fallbacks) |
| Caching and scheduled work | GitWicket (six-hour Redis cache), NetaBoard (Vercel Cron for briefs and refreshes) |
| Verification beyond "it runs" | NetaBoard (unit tests plus a script that checks a live deployment is one coherent build), SentiFi (pytest) |

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

## Tech Stack

| | |
|:--|:--|
| **Languages** | Python · JavaScript · TypeScript · C++ · Java · SQL |
| **Backend** | Flask · FastAPI · Node.js · Express · REST APIs |
| **Frontend** | Next.js · Vanilla JS · Tailwind CSS |
| **AI / ML** | LLM APIs (Groq, Gemini) · Ollama · NLP · Scikit-learn · TensorFlow |
| **Databases** | PostgreSQL · SQLite · Supabase · Redis |
| **Infrastructure** | Docker · AWS · VPS · Vercel · Render |
| **Tools** | Git · GitHub · VS Code · Jupyter · Colab |

<br/>

<sub>**Recognition:** Konam AI Fellowship (selected) · AWS Academy Graduate, Cloud Foundations · Google Developers × AICTE AI-ML Virtual Internship · Altair × AICTE Data Science Master Internship · Honeywell AI Certificate</sub>

<div align="center"><img src="./assets/divider.svg" alt="" width="100%"/></div>

<div align="center">
  <sub>
    <a href="mailto:ashmitsingh702@gmail.com">Email</a> &nbsp;·&nbsp;
    <a href="https://www.linkedin.com/in/ashmitvsingh/">LinkedIn</a> &nbsp;·&nbsp;
    <a href="https://ashmit-702.github.io/portfolio/">Portfolio</a>
  </sub>
</div>
