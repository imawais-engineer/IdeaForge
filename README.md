# IdeaForge: Zero-to-One Second Brain

**USAII Hackathon 2026 - Undergraduate Track**  
**Project**: The Second Brain  
**Direction**: Zero To One Builder  

![IdeaForge Hero](https://drive.google.com/uc?id=13lg5mwRhYElqEnSaZHcsySzbRojlW9f7)

**Modern AI Second Brain Coach** | Turn Vague Ideas Into Actionable First Steps

## 🎥 Demo Video

[![IdeaForge Demo Video](https://img.youtube.com/vi/g2tj21erVDQ/maxresdefault.jpg)](https://youtu.be/g2tj21erVDQ)

**Watch the full demo** → [YouTube: IdeaForge: Zero-to-One Builder Challenge | Made in n8n](https://youtu.be/g2tj21erVDQ)

## 🚀 Try It Live

**[Try IdeaForge Now](https://n8nio.imawais.engineer/webhook/dd8709a3-30c4-4a2b-8386-7c5a2e4e2459/chat)**

*Modern dark UI with cyan accents — mobile-friendly chat experience*

## Inspiration

The hackathon brief for **"Build the Second Brain for Real Life"** deeply resonated with us. As college students and aspiring creators, we saw talented peers with strong ideas — campus startups, class projects, and personal ambitions — frequently stuck in **execution paralysis**.

Modern life overwhelms us with information, hidden tradeoffs, and constant context switching. Most tools either oversimplify (generic task lists) or add more noise. **IdeaForge** fills this gap by acting as a thoughtful **reasoning partner** — helping users move from vague ideas to structured, realistic plans with clear first steps.

## What It Does

**IdeaForge** is an AI-powered Second Brain Coach for college students, recent graduates, aspiring founders, and career-switchers.

### Core Features
- **Idea Clarification** — Refines vague concepts with personal context
- **Assumptions & Risks Analysis** — Surfaces key assumptions with confidence scores (Low/Medium/High)
- **Structured Roadmaps** — Phased execution plans + realistic 30-day action plans
- **Life Balance Focus** — Built-in guidance on studies, burnout prevention, and sustainable execution
- **Human Decision Moment** — Every response ends with clear disclaimers: *final decisions always remain with you*
- **Document Assistant** — Upload resumes, cover letters, or proposals → professional feedback or Google Docs generation

![Main Agent Workflow](https://drive.google.com/uc?id=1yrCHeDvgypUiychkT53CDAK57HFhGl0g)

## How We Built It

We followed a structured SDLC approach and built a functional, reliable system in **n8n**.

### Architecture Highlights
- **Chat Interface** with custom CSS and welcome screen
- **Main AI Agent** powered by Groq (`gpt-oss-120b`) with strict system prompt
- **RAG Pipeline** — Pinecone vector store + Hugging Face embeddings (loaded with hackathon guidelines & SRS)
- **MongoDB** — Persistent chat memory
- **Document Branch** — File upload handling + Google Docs automation
- **Responsible AI Guardrails** — Embedded throughout (uncertainty framing, risks, mitigations, human-in-the-loop)

![RAG & Guardrails Setup](https://drive.google.com/uc?id=1fLxffjypqWRuyFzj2hrT1Q-zwkeRjQbd)  
![Document Agent Branch](https://drive.google.com/uc?id=19sJ6Zq5KbElJPV3jEAiUVNLVSjfTWLBI)

**Tech Stack**:
- n8n (orchestration)
- Groq + MiniMax models
- Pinecone + Hugging Face
- Google Drive/Docs
- MongoDB

## Project Resources

**Full Google Drive Folder**: [https://drive.google.com/drive/folders/1FLcqa7huEboNHa9eUjoAjnaJwAvy06M_](https://drive.google.com/drive/folders/1FLcqa7huEboNHa9eUjoAjnaJwAvy06M_?usp=sharing)

### Key Files
- **Workflow JSON** — [Start-up Ideas Generator.json](https://drive.google.com/file/d/1Gp-PoUcGmcWKKouX9KIcs4iaAaCMJWm1/view?usp=drive_link)
- **RAG Global Instructions** — [Download PDF](https://drive.google.com/file/d/1fLxffjypqWRuyFzj2hrT1Q-zwkeRjQbd/view?usp=drive_link)
- **SRS Document** — [Download PDF](https://drive.google.com/file/d/1Mx0sKlhdBv7akPP7xMK_7ox-maCzeKj3/view?usp=drive_link)
- **UI Screenshot** — [View](https://drive.google.com/file/d/13lg5mwRhYElqEnSaZHcsySzbRojlW9f7/view?usp=drive_link)
- **Main Agent** — [View](https://drive.google.com/file/d/1yrCHeDvgypUiychkT53CDAK57HFhGl0g/view?usp=drive_link)
- **RAG Setup** — [View](https://drive.google.com/file/d/1fLxffjypqWRuyFzj2hrT1Q-zwkeRjQbd/view?usp=drive_link)
- **Document Agent** — [View](https://drive.google.com/file/d/19sJ6Zq5KbElJPV3jEAiUVNLVSjfTWLBI/view?usp=drive_link)

## Challenges & Accomplishments

**Challenges**:
- Deep prompt engineering for structured reasoning (avoiding generic lists)
- Reliable RAG + file handling
- Balancing depth with scannable, encouraging outputs

**Proud Achievements**:
- Fully functional system matching hackathon mandatory response structure
- Strong Responsible AI implementation
- Clean, professional UI + seamless Google Docs export
- Dual-purpose tool (Idea Coaching + Document Assistant)

## What We Learned

Building great AI tools is more about **structuring thinking** and enforcing disciplined reasoning than raw model power. Responsible AI guardrails and human-in-the-loop design significantly increase trustworthiness.

## What's Next

- Full multi-agent orchestration (Clarifier, Risk Analyzer, Planner, Simulator, Orchestrator)
- Calendar & Notion integrations
- Progress tracking & feedback loops
- Open-source templates for common student scenarios
- Voice input and collaborative team features

---
---

**Made with ❤️ for USAII Hackathon 2026**

*Helping the next generation of students and creators move from vague ideas to real execution.*

### Built by
**Muhammad Awais** & **Muhammad Zaid**

### Submission
Submitted on Devpost → [View Project on Devpost](https://devpost.com/software/neuronic-ai)

---
