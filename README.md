Inspiration
The hackathon brief for "Build the Second Brain for Real Life" deeply resonated with us. As college students and aspiring creators, we repeatedly witnessed talented peers with promising ideas — campus startups, innovative class projects, and personal ambitions — get stuck in execution paralysis.

Modern life brings overwhelming information, hidden tradeoffs, and constant mental switching, yet most tools either oversimplify (basic pros/cons or task lists) or overwhelm users. We were inspired to build a tool that fills this gap by helping users reason effectively, turning vague early-stage ideas into realistic, actionable plans.

What it does
IdeaForge: Zero-to-One Second Brain is an AI-powered multi-agent system that helps college students, recent graduates, aspiring founders, and career-switchers transform vague ideas into structured execution plans.

Users provide a natural language description of their idea along with personal constraints. The system clarifies the idea, surfaces key assumptions and risks, generates a tailored milestone roadmap (including 30/60/90-day views or MVP stages), simulates scenarios with tradeoffs, and delivers a concrete first real step.

Every output includes uncertainty framing, confidence indicators, and clear disclaimers — ensuring the tool supports thinking rather than replacing human judgment.

How we built it
We followed a structured software engineering approach aligned with the hackathon’s emphasis on thoughtful design.

Key Components:

A 5-agent architecture built in n8n:
Idea Clarifier
Assumption & Risk Analyzer
Milestone Planner
Scenario Simulator & Tradeoff Modeler
Synthesis & Action Orchestrator
Powered by Grok and Claude 3.5 Sonnet for advanced reasoning chains.
Integrated with Notion, Google Docs, and Google Calendar for seamless export and immediate action.
Comprehensive Responsible AI guardrails embedded at every stage.
The entire workflow creates a coherent pipeline:
Input → Multi-Agent Reasoning → Structured Output → User Decision → Action.

Challenges we ran into
Designing agents that perform deep reasoning without generating generic task lists was technically and prompt-engineering intensive.
Balancing rich analysis with user-friendly, non-overwhelming outputs required multiple iterations.
Ensuring strong uncertainty representation and human-in-the-loop controls while maintaining practicality within the tight one-week build window.
Accomplishments that we're proud of
Built a fully functional multi-agent system in n8n that demonstrates a clear input → reasoning → output → action flow.
Created 15 realistic problem statements and detailed blueprints that directly map to target user needs.
Implemented robust Responsible AI features including risk matrices, confidence scores, multiple scenarios, and explicit human control points.
Delivered a practical tool that genuinely helps users move from confusion to meaningful first steps.
What we learned
We learned that effective AI for decision support is less about automation and more about structuring thinking and surfacing blind spots. Designing with Responsible AI from the start significantly improved the quality and trustworthiness of the system. We also gained deep appreciation for multi-agent orchestration and the importance of transparency in AI systems.

What's next for IdeaForge: Zero-to-One Second Brain
We plan to expand the tool with user feedback loops, more integration options (calendar reminders, progress tracking), and additional templates for common student scenarios. Long-term, we aim to make it a widely accessible open-source Second Brain for young creators and professionals, potentially adding voice input and collaborative team modes.
