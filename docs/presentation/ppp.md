---
marp: true
theme: default
paginate: true
header: "ASE285 Individual Project - PPP"
footer: "Joshua | February 2026"
---

# Individual Project

## ChatGPT-like Cross-Platform Application

**Joshua**
ASE285 - Software Engineering

---

# Agenda

1. Project Overview
2. Problem Domain
3. Features & Requirements
4. Architecture & Data Model
5. Test Strategy
6. Sprint Progress & Burndown
7. Demo
8. Q&A

---

# Project Overview

## ChatGPT-like Cross-Platform Web/Desktop Application

- **Goal:** Build an AI chat interface application
- **Platform:** Web and Desktop (cross-platform)
- **Tech Stack:** React 18, Redux Toolkit, Vite, Electron, OpenAI SDK

---

# Problem Domain

## Students struggle with:

- Limited access to AI assistance for learning
- Need for cross-platform accessibility (web and desktop)
- Managing multiple conversations and context
- Organizing AI interactions for different tasks

## Our Solution:

- Cross-platform ChatGPT-like application
- Persistent conversation history with localStorage
- Intuitive interface for managing multiple chat sessions
- Seamless integration with OpenAI API

---

# Features & Requirements

## Functional Requirements

| #   | Feature                 | Requirements | Status |
| --- | ----------------------- | ------------ | ------ |
| 1   | Chat Interface          | 5            | 🔄     |
| 2   | Conversation Management | 4            | 🔄     |
| 3   | OpenAI Integration      | 3            | 🔄     |
| 4   | State Management        | 3            | 🔄     |
| 5   | Cross-Platform Support  | 2            | 🔄     |

**Total:** 5 Features, 17 Requirements

Link: [Features & Requirements Details](../features/overall.md)

---

# Non-Functional Requirements

- 🔄 Web application support
- 🔄 Desktop application support (Electron)
- 🔄 Cross-platform compatibility (Windows, Mac, Linux)
- 🔄 Responsive UI design
- 🔄 Local data persistence (localStorage)
- 🔄 Real-time AI communication
- 🔄 Secure API key management

---

# Architecture

- **Frontend:** React 18 with Redux Toolkit
- **API Integration:** OpenAI SDK (openaiService.js)
- **Desktop:** Electron wrapper
- **Storage:** localStorage for persistence
- **Build Tool:** Vite for fast development

Link: [System Architecture](../architecture/system_architecture.md)

---

# Data Model

- **Conversation**: id, title, createdAt, messages array
- **Message**: id, content, role (user/assistant), timestamp
- **Relationship**: 1:N (Conversation has many Messages)
- **Storage**: Persisted to localStorage

Link: [Data Model Diagram](../architecture/data_model.md)

---

# Test Strategy

| Test Type         | Count | Coverage |
| ----------------- | ----- | -------- |
| Unit Tests        | 0     | 0%       |
| Integration Tests | 0     | 0%       |
| E2E Tests         | 0     | 0%       |
| Acceptance Tests  | 0     | 0%       |

**Status:** Tests will be implemented throughout Sprint 1 and Sprint 2

Links:

- [Unit Tests](../../tests/unit_tests/)
- [Integration Tests](../../tests/integration_tests/)
- [E2E Tests](../../tests/e2e_tests/)
- [Acceptance Tests](../../tests/acceptance_tests/)

---

# Sprint 1 Progress (Weeks 4-8)

## Planned Features:

- 🔄 Feature 1: Chat Interface (0/5 requirements)
- 🔄 Feature 2: Conversation Management (0/4 requirements)
- 🔄 Feature 3: OpenAI Integration (0/3 requirements)
- 🔄 Feature 4: State Management (0/3 requirements)
- 🔄 Feature 5: Cross-Platform Support (0/2 requirements)

## Planned Deliverables:

- [ ] Project setup and architecture design
- [ ] React components (App, Dashboard, Chat, Sidebar)
- [ ] Redux store configuration
- [ ] OpenAI service integration
- [ ] Data model design
- [ ] System architecture documentation
- [ ] Test suite implementation
- [ ] Electron desktop application

## Metrics:

- **Features burn down rate:** 0/5 finished (0%)
- **Requirements burn down rate:** 0/17 finished (0%)
- **LoC:** 0 (Source code)
- **Tests:** 0 unit tests, 0 integration tests, 0 e2e tests

## Links:

- [Source Code](../../src/)
- [Documentation](../../docs/)
- [Individual Progress](../../individual/joshua/progress.md)

# Sprint 2 Plan (Weeks 9-16)

## Goals:

- [ ] Complete all 5 features and 17 requirements
- [ ] Implement full test suite (unit, integration, e2e, acceptance)
- [ ] Build and deploy Electron desktop application
- [ ] Implement conversation management features
- [ ] Build OpenAI integration with error handling
- [ ] Performance optimization
- [ ] Complete documentation

## Timeline:

- Week 9-10: Project setup, React components, basic chat interface
- Week 11-12: OpenAI integration, conversation management
- Week 13-14: Electron desktop app, state management, tests
- Week 15-16: Final features, testing, documentation, deployment

---

# Demo

## Application Preview

**Status:** Development begins in Sprint 1

**Planned Demo:**

- ChatGPT-like interface with sidebar
- Real-time AI conversation
- Multiple conversation management
- Cross-platform (Web + Desktop)

---

# Summary

## Current Status:

- 🔄 Planning phase complete
- 🔄 Architecture and data model designed
- 🔄 Technology stack selected
- 🔄 Feature requirements defined
- 🔄 Ready to begin Sprint 1 development

## Sprint 1 Focus:

- Set up development environment
- Build core React components
- Implement OpenAI integration
- Create conversation management
- Begin test implementation

---

# Q&A

## Questions?

**Repository:** <https://github.com/Jolteer/ASE285_Individual>

**Quick Links:**

- [Documentation](https://github.com/Jolteer/ASE285_Individual/tree/main/docs)
- [Source Code](https://github.com/Jolteer/ASE285_Individual/tree/main/src)
- [Tests](https://github.com/Jolteer/ASE285_Individual/tree/main/tests)
- [Individual Progress](https://github.com/Jolteer/ASE285_Individual/blob/main/individual/joshua/progress.md)

---

# Thank You!

**Contact:**

- GitHub: Jolteer
- Project: ASE285_Individual
