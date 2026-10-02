<img src="assets/header.svg" width="100%" alt="Leo Yeh — AI product builder · founder"/>

<p align="center">
  <a href="https://www.linkedin.com/in/leo-yeh-37952a149/"><img src="https://img.shields.io/badge/LinkedIn-Leo%20Yeh-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:leo1125s@gmail.com"><img src="https://img.shields.io/badge/Email-leo1125s%40gmail.com-14213d?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://img.shields.io/badge/Based%20in-Taipei%2C%20Taiwan-e9a23b?style=flat-square" alt="Taipei, Taiwan"/>
</p>

I come from the business side of B2B SaaS (business development, customer success and CRM implementation) and I build AI products myself. I take a product from the problem to production: system design, LLM pipelines, backend, payments, cloud deployment, testing and monitoring.

I work AI-first with Claude Code, but treat the output like production software: typed code, migrations, CI/CD, observability and large automated test suites.

<br/>

## ✨ What I Do

<img src="assets/capabilities.svg" width="100%" alt="AI Agents · Web Products · Chatbots · Data & Cloud"/>

<br/>

## 🚀 Featured Builds

<table>
<tr>
<td width="50%" valign="top">

### [TripDayNDay](https://www.tripdaynday.com/)
<sub>**FOUNDER & BUILDER** · MULTILINGUAL AI ASSISTANT ON LINE</sub>

Users send a photo, voice note or text in LINE and get a plain-language answer, with optional spoken replies. Built for older adults, so there's no app to install.

- **Multimodal AI:** Gemini 2.5 Flash reads photos (menus, signs, labels); Google Cloud TTS speaks replies
- **Four languages, one backend:** Traditional Chinese, English, Japanese and Thai LINE channels served by a single FastAPI service
- **Full product stack:** Stripe subscriptions and paywall, referral tracking, promo codes, LIFF web front end, auto-generated travel recap videos (moviepy + ffmpeg)
- **Production engineering:** async SQLModel on Cloud SQL PostgreSQL, Alembic migrations, Docker → GitHub Actions → Cloud Run, Sentry + OpenTelemetry tracing
- **2,400+ automated tests** across the codebase

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/> <img src="https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini"/> <img src="https://img.shields.io/badge/Cloud%20Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Cloud Run"/> <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>

</td>
<td width="50%" valign="top">

### [Structaly](https://structaly.com/)
<sub>**FOUNDER & BUILDER** · AI ORDER-TAKING FOR B2B SUPPLIERS</sub>

Small food and hardware suppliers get orders as casual messages in LINE group chats. Structaly turns them into structured, confirmed orders without asking customers to change how they write.

- **Hybrid parsing engine:** a rule-based gate filters out non-orders at zero LLM cost → the LLM only *copies* text spans (temperature 0) → deterministic code matches items, quantities and dates
- **Design backed by evals:** a golden test set showed LLMs "deciding" orders invented or dropped them, so the model never makes the call
- **"Flag, never guess":** anything uncertain is marked for human review instead of filled with a plausible value
- **Photo orders:** one Vision call both classifies the image and transcribes it
- **Self-learning catalog:** new items are recorded automatically but only trusted after human confirmation
- **Multi-tenant safety:** every database query requires a supplier ID, so there's no way to read across tenants. 400+ tests run in ~3 seconds

<img src="https://img.shields.io/badge/LLM%20pipeline-0f766e?style=flat-square" alt="LLM pipeline"/> <img src="https://img.shields.io/badge/Vision%20OCR-0f766e?style=flat-square" alt="Vision OCR"/> <img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/> <img src="https://img.shields.io/badge/LINE%20LIFF-06C755?style=flat-square&logo=line&logoColor=white" alt="LINE LIFF"/> <img src="https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/>

</td>
</tr>
<tr>
<td colspan="2" valign="top">

### [vediocut](https://github.com/leoai123/vediocut-case-study) &nbsp;<sub>📖 CASE STUDY</sub>
<sub>**BUILDER** · TRANSCRIPT-FIRST AI VLOG EDITOR</sub>

Turns a pile of handheld phone clips into a narrative vlog by understanding what was said first, then deciding how to cut, the way a human editor works. Iterated on nine real shoots.

- **Local speech recognition:** whisper.cpp + voice-activity detection + word-level timestamps, fully on-device
- **Correction with world knowledge, not glossaries:** the LLM infers region and topic from the transcript to fix misheard names. In testing this fixed twice as many errors as a hand-built glossary
- **"Radio edit" first:** the story must make sense with the picture off, and cuts land only at sentence ends
- **LLM decides, rules verify:** the edit plan must pass a deterministic validation gate before anything renders
- **B-roll via Chinese-CLIP with human review:** similarity scores alone mislead on similar-looking footage
- **Make failures loud:** silent failures were the costliest bugs, so each one became an explicit check

<img src="https://img.shields.io/badge/whisper.cpp-14213d?style=flat-square" alt="whisper.cpp"/> <img src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude"/> <img src="https://img.shields.io/badge/Chinese--CLIP-0f766e?style=flat-square" alt="Chinese-CLIP"/> <img src="https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white" alt="FFmpeg"/> <img src="https://img.shields.io/badge/librosa-0f766e?style=flat-square" alt="librosa"/> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>

</td>
</tr>
</table>

<br/>

## 🧩 Other Work

| Project | What I built |
|---|---|
| **AI agency for small businesses** | AI agents that automate marketing, sales outreach and back-office workflows. Multilingual B2B websites on Next.js + Sanity CMS, set up so clients edit content themselves. |
| **B2B sourcing platform** | Pipelines that pull manufacturers' full product catalogs from websites and PDFs (including OCR for scanned files) into a structured, searchable supplier database. Next.js + Prisma. |
| **Generative-AI avatar startup** | Led product: roadmap, pricing and partnerships for a virtual-influencer platform. |
| **AI local newsletter** | An AI-edited local newspaper, generated and delivered as a newsletter, one edition per city. |
| **Commuter map** | A map with a social layer, running on Cloudflare Workers. |
| **LINE group game** | A puzzle game played inside LINE group chats with a weekly leaderboard (LIFF + Phaser + Hono). |

<br/>

## 🧭 How I Build

<table>
<tr>
<td width="33%" valign="top">

**⚙️ Deterministic first, LLM second**

Rules handle what rules can. The model only does the part that truly needs language understanding, which keeps cost low and behavior predictable.

</td>
<td width="33%" valign="top">

**🧪 Prove it with evals**

Design choices come from test sets, not intuition. Every important behavior is pinned by an automated test.

</td>
<td width="33%" valign="top">

**🔒 Safe by construction**

Tenant isolation, cost limits and product boundaries are enforced in code, so a future change can't quietly break them.

</td>
</tr>
</table>

<br/>

## 🛠 Toolkit

**AI** &nbsp;
<img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=anthropic&logoColor=white" alt="Claude Code"/>
<img src="https://img.shields.io/badge/Gemini%20API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white" alt="Gemini"/>
<img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI"/>
<img src="https://img.shields.io/badge/AI%20agent%20design-0f766e?style=flat-square" alt="AI agent design"/>
<img src="https://img.shields.io/badge/LLM%20evals-0f766e?style=flat-square" alt="LLM evals"/>
<img src="https://img.shields.io/badge/Speech%20%26%20vision%20models-0f766e?style=flat-square" alt="Speech & vision models"/>

**Backend** &nbsp;
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/SQLModel%20%2B%20Alembic-14213d?style=flat-square" alt="SQLModel + Alembic"/>
<img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white" alt="Stripe"/>
<img src="https://img.shields.io/badge/LINE%20Messaging%20API-06C755?style=flat-square&logo=line&logoColor=white" alt="LINE"/>

**Frontend** &nbsp;
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
<img src="https://img.shields.io/badge/Sanity-F03E2F?style=flat-square&logo=sanity&logoColor=white" alt="Sanity"/>
<img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>

**Data & Cloud** &nbsp;
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud"/>
<img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
<img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" alt="Sentry"/>
<img src="https://img.shields.io/badge/Metabase-509EE3?style=flat-square&logo=metabase&logoColor=white" alt="Metabase"/>

**Business** &nbsp;
<img src="https://img.shields.io/badge/Go--to--market-14213d?style=flat-square" alt="GTM"/>
<img src="https://img.shields.io/badge/Pricing-14213d?style=flat-square" alt="Pricing"/>
<img src="https://img.shields.io/badge/CRM%20implementation-14213d?style=flat-square" alt="CRM implementation"/>
<img src="https://img.shields.io/badge/Salesforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white" alt="Salesforce"/>
<img src="https://img.shields.io/badge/HubSpot-FF7A59?style=flat-square&logo=hubspot&logoColor=white" alt="HubSpot"/>

<br/>

<p align="center"><sub>⛰️ Mountaineering (38 of Taiwan's Top 100 Peaks) · 🌊 Free diving</sub></p>
