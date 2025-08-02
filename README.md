# 🧠 Agentic Agile Coach

> A self-improving, multi-agent AI system for evaluating Agile user stories and sprint backlogs — deeply integrated with Jira and your team’s real-world delivery context.

---

## 🚀 Overview

**Agentic Agile Coach** is an experimental, AI-native product that helps Agile teams write better
user stories, ensure sprint readiness, and continuously improve how work is planned and delivered.

The system uses a team of intelligent agents to evaluate, improve, and align Jira backlogs with
your sprint goals, OKRs, roadmap, and historical velocity.

⚡ MVP runs via CLI.  
🧩 Full release integrates seamlessly with Jira via Forge.

---

## 🔍 Key Features

- **User Story Quality Scoring**  
  Evaluates stories across customizable criteria with 0–10 scoring + improvement advice.

- **Sprint Readiness Analysis**  
  Detects blockers, risks, misalignments, gaps, and suggests resolution steps.

- **Conversational Clarification Agent**  
  Automatically identifies and resolves missing or ambiguous information.

- **RAG-Enhanced Context Retrieval**  
  Pulls from OKRs, roadmap, docs, test results, and velocity history to evaluate completeness.

- **Backlog Editing & Planning Advisor**  
  Can recommend, remove, or rewrite stories to keep the sprint on track.

- **Self-Learning Feedback Loop**  
  Learns from past sprint performance and user feedback to improve future assessments.

---

## 🧰 Tech Stack

| Component       | Description                                  |
|-----------------|----------------------------------------------|
| **LangGraph**   | Multi-agent orchestration                    |
| **LiteLLM**     | LLM gateway abstraction                      |
| **Weaviate**    | Vector DB for RAG context                    |
| **Jira API**    | Backlog access and integration               |
| **CTRF Parser** | Structured test result ingestion             |
| **CLI**         | MVP UX (terminal-based)                      |
| **Jira Forge**  | Final UX (native Jira integration)           |

---

## 📁 Repository Structure

agentic-agile-coach/
├── src/
│ ├── agents/ # Specialized agent implementations
│ ├── core/ # LangGraph workflow, planner logic
│ ├── parsers/ # CTRF, OKR, roadmap, etc.
│ └── cli/ # CLI entry point and commands
├── docs/
│ ├── VISION.md # Product vision and mission
│ ├── ARCHITECTURE.md # System architecture diagram and rationale
│ ├── ROADMAP.md # Product roadmap and milestones
│ └── UX.md # UX design for MVP and Forge app
├── .coachrc # Config file for CLI mode
├── README.md # You are here
└── requirements.txt # Python dependencies

---

## 📦 Getting Started

### Prerequisites

- Python 3.13+
- Access to OpenAI or Claude via LiteLLM
- Jira API token with project read/write permissions

### Installation

```bash
git clone https://github.com/your-org/agentic-agile-coach.git
cd agentic-agile-coach
pip install -r requirements.txt
```

### CLI Usage Example

```bash
# Score a user story
coach analyze-story STORY-123

# Check sprint readiness
coach check-backlog SPRINT-42

# Clarify a problematic story
coach clarify STORY-456
```

## 📌 Roadmap

We’re starting small, but moving fast. Check the full 📄 ROADMAP for milestone details.

## 🛡 Security & Privacy

This system operates on sensitive delivery and product data. See 📄 ARCHITECTURE.md for security,
data protection, and resilience considerations.

## 💬 Feedback & Contributions

We welcome issues, ideas, and pull requests.

For major features or changes, please open a discussion first.

## 🧠 Related Docs

- [Product Vision](docs/vision.md)
- [System Architecture](docs/architecture.md)
- [Product Roadmap](docs/roadmap.md)
- [UX Design](docs/architecture.md#-frictionless-user-experience)

## 📜 License

MIT License — see LICENSE for full details.