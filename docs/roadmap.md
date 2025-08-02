# Roadmap

## 🚩 Milestone 1: MVP – Core Workflow

Establish the foundation for an agentic AI system capable of evaluating user stories and sprint
backlogs, interacting with users, and offering quality insights.

### ✅ Key Deliverables:

- System architecture with LangGraph and LiteLLM
- Core agent scaffolding:
  - User Story Evaluator Agent (v1)
  - Sprint Readiness Assessor Agent (v1)
  - Conversational Validator Agent
  - Context Retriever Agent (RAG v1) using Weaviate
  - Static assessment criteria
  - CLI or minimal UI for input/output
  - Working demo using real sprint backlog

## 🚩 Milestone 2: Self-Learning Foundations

Begin collecting and incorporating team feedback and historical sprint outcomes into the scoring and analysis models.

### ✅ Key Deliverables:

- Feedback Integrator Agent
  - Learns from story scores vs actual delivery outcomes
  - Tracks velocity drift, rework, and carryover
- Enhancement of scoring heuristics based on data
- RAG indexing of sprint reports, retros, delivery logs
- Story evaluation tuning based on team-specific trends

## 🚩 Milestone 3: Contextual Intelligence & Backlog Automation

Deepen system understanding of sprint planning context and allow for intelligent backlog updates and story generation.

### ✅ Key Deliverables:

- Improved RAG: Load OKRs, roadmap, tech specs, dependencies
- Conversational backlog editing (add, remove, modify stories)
- Backlog validation rules:
  - Sequencing
  - Risk clustering
  - Goal alignment
- Draft new user stories based on gaps or roadmap needs

## 🚩 Milestone 4: Adaptive Multi-Team Coaching

Support multiple teams and tailor evaluations to their domain, maturity, and velocity trends.

### ✅ Key Deliverables:

- Team profiles (personas)
  - Customize scoring weights and suggestions
- Cross-sprint evaluation
  - Compare delivery trends across teams
- Aggregated sprint readiness and quality reports

## 🚩 Milestone 5: Autonomous Planning Advisor

Extend the system to proactively guide sprint planning and backlog shaping based on strategic intent and historical learning.

### ✅ Key Deliverables:

- Autonomous suggestions:
  - Story prioritization
  - Risk surfacing
  - Story sequencing
  - Sprint success prediction engine
- Executive reports on:
  - Sprint readiness score
  - Alignment to OKRs/roadmap
  - Delivery risk forecasts
