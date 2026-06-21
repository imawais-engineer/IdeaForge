## Inspiration
The hackathon brief for **"Build the Second Brain for Real Life"** deeply resonated with us. As college students and aspiring creators, we repeatedly saw talented peers with promising ideas — campus startups, innovative class projects, and personal ambitions — get stuck in execution paralysis. Modern life brings overwhelming information, hidden tradeoffs, and constant mental switching, yet most tools either oversimplify (basic pros/cons or generic task lists) or overwhelm users. We set out to build a practical tool that fills this gap by acting as a **reasoning partner** — helping users move from vague ideas to structured, realistic plans with clear first steps.

## What it does
**IdeaForge: Zero-to-One Second Brain** is an AI-powered Second Brain Coach that helps college students, recent graduates, aspiring founders, and career-switchers transform vague ideas into actionable execution plans.

Users describe their idea in natural language along with personal context (studies, time constraints, resources, etc.). The system:
- Clarifies and refines the idea
- Surfaces key assumptions and risks with confidence levels
- Delivers a structured execution roadmap (including a realistic 30-day action plan)
- Emphasizes study/life balance and burnout prevention
- Always ends with a clear **Human Decision Moment**

Every response follows a consistent, scannable format and includes responsible AI elements: uncertainty framing, confidence scores (Low/Medium/High), tradeoffs, and explicit disclaimers that the final decisions remain with the user.

It also includes a **Document Assistant** mode where users can upload resumes, cover letters, or other documents to get professional feedback or generate improved versions directly into Google Docs.

## How we built it
We built a functional, production-ready workflow in **n8n** following a thoughtful software engineering approach:

**Core Components:**
- **Intelligent Chat Interface** with custom styling and conversation memory (MongoDB)
- **Powerful Main Agent** (`IdeaForge`) powered by Groq (gpt-oss-120b) with a carefully engineered system prompt enforcing the mandatory response structure
- **RAG System** using Pinecone vector database + Hugging Face embeddings, pre-loaded with hackathon guidelines and SRS documents for consistent, context-aware responses
- **Document Processing Branch**: Handles file uploads (PDFs, DOCX), analyzes them, and creates/improves documents using Google Docs integration
- **Responsible AI Guardrails** embedded directly into the agent prompts

The architecture creates a clean pipeline:  
**Chat Input → Context Retrieval (RAG) → Structured Reasoning → Formatted Output → Actionable Next Step**

## Challenges we ran into
- Crafting prompts that produce deep reasoning instead of generic task lists required significant iteration.
- Balancing comprehensive analysis with concise, student-friendly outputs.
- Implementing robust file handling and Google Docs automation while keeping the workflow reliable.
- Ensuring strong uncertainty representation and human-in-the-loop principles without making the experience feel overly cautious.

## Accomplishments that we're proud of
- Delivered a fully working, responsive AI coach that follows the exact response structure required by the hackathon brief.
- Successfully implemented RAG with relevant project documents for grounded, consistent responses.
- Built a dual-purpose system: idea-to-execution coaching + professional document assistance.
- Embedded Responsible AI practices (confidence scores, risk/mitigation framing, explicit human decision points) throughout.
- Created a clean, modern chat UI with custom CSS and seamless Google Docs export.

## What we learned
We learned that building effective decision-support AI is more about **structuring thinking** and enforcing disciplined reasoning than about raw model power. Prompt engineering for consistency and responsibility is just as important as the underlying technology. We also gained hands-on experience with n8n orchestration, vector databases (Pinecone), and integrating AI with productivity tools.

## What's next for IdeaForge
We plan to evolve IdeaForge by:
- Expanding into a true multi-agent system (Clarifier, Risk Analyzer, Planner, Simulator, Orchestrator)
- Adding more integrations (Google Calendar, Notion, export to PDF/Word)
- Implementing user feedback loops and progress tracking
- Creating specialized templates for common student scenarios (career decisions, side hustles, class projects to pilots)
- Making the project open-source so other students can build upon it

IdeaForge is a practical step toward a real "Second Brain" for the next generation of creators and founders.
