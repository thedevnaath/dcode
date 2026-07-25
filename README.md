<div align="center">

# DCODE

### *It has already begun.*

**A global psychological horror mystery driven by a single shared countdown.**

---

> *The countdown belongs to everyone. The mystery belongs to no one.*

<br>

![Project Status](https://img.shields.io/badge/Status-Planning-orange)
![Platform](https://img.shields.io/badge/Platform-Web-blue)
![Type](https://img.shields.io/badge/Genre-ARG%20%7C%20Psychological%20Horror-black)
![Frontend](https://img.shields.io/badge/Frontend-HTML%20%7C%20CSS%20%7C%20JavaScript-red)
![Hosting](https://img.shields.io/badge/Hosting-GitHub%20Pages-success)
![Countdown](https://img.shields.io/badge/Countdown-Global-important)

---

### ⚠️ NOTICE

This repository currently contains the **planning, architecture and implementation** of **DCODE**.

The mystery itself is **not** stored inside this repository.

Critical secrets, final puzzle solutions, verification methods, reward assets and production infrastructure are intentionally excluded from version control.

---

</div>

# Table of Contents

- [Overview](#overview)
- [Vision](#vision)
- [Core Philosophy](#core-philosophy)
- [Project Objectives](#project-objectives)
- [Why DCODE Exists](#why-dcode-exists)
- [Design Principles](#design-principles)
- [Core Experience](#core-experience)
- [Feature Overview](#feature-overview)

---

# Overview

**DCODE** is a web-based psychological horror experience that combines elements of:

- Interactive storytelling
- Cryptography
- Alternate Reality Games (ARGs)
- Community collaboration
- Global participation
- Psychological suspense

Unlike conventional countdown websites, DCODE is designed as a **living mystery**.

Visitors do not simply observe a timer.

They become participants in an evolving investigation whose rules are intentionally undisclosed.

The project continuously changes over time, revealing new clues, hidden systems and increasingly complex puzzles while maintaining a single central question:

> **What happens when the countdown reaches zero?**

The answer is never explicitly presented.

It must be earned.

---

# Vision

Create an internet experience that people remember years after encountering it.

DCODE is intended to become more than a website.

It should become:

- a community
- an investigation
- a long-running internet mystery
- a collaborative puzzle
- a psychological experience

The project should encourage visitors to return repeatedly—not because they are told to, but because they feel there is always something they have missed.

---

# Core Philosophy

Most websites provide information.

DCODE deliberately withholds it.

Every design decision should increase one or more of the following emotions:

| Emotion | Purpose |
|---------|----------|
| Curiosity | Encourage exploration |
| Uncertainty | Prevent predictable outcomes |
| Suspense | Build long-term anticipation |
| Discovery | Reward observation |
| Collaboration | Encourage community investigation |
| Satisfaction | Make discoveries meaningful |

If a feature does not strengthen at least one of these emotions, it should be reconsidered.

---

# Project Objectives

The long-term objectives of DCODE are:

| Objective | Description |
|------------|-------------|
| Global Participation | Create a single mystery experienced by everyone simultaneously. |
| High Replay Value | Encourage users to revisit regularly. |
| Community Discussion | Inspire theories, investigations and collaborative decoding. |
| Long-Term Engagement | Sustain interest over months or years through evolving content. |
| Meaningful Rewards | Ensure discoveries feel genuinely valuable. |
| Technical Excellence | Build a reliable, scalable and maintainable platform. |

---

# Why DCODE Exists

Modern countdown websites are predictable.

Visitors know exactly what they are counting toward.

DCODE intentionally removes that certainty.

Instead of answering questions, it creates them.

Rather than announcing an event, it constructs an experience where the unknown becomes the primary attraction.

The countdown is not the destination.

It is the mechanism through which the mystery unfolds.

---

# Design Principles

Every future feature should follow these principles.

| Principle | Description |
|-----------|-------------|
| Mystery First | Never explain more than necessary. |
| Story Through Discovery | Users uncover the narrative themselves. |
| Community Over Individuals | Collaboration should naturally emerge. |
| Minimalism | Remove visual noise. Focus attention on what matters. |
| Psychological Horror | Create discomfort through uncertainty rather than shock. |
| Authenticity | Every clue should feel intentional and meaningful. |
| Longevity | Systems should support years of continuous evolution. |

---

# Core Experience

At its simplest, the visitor experience follows this pattern:

```text
Visitor arrives
        │
        ▼
Sees the countdown
        │
        ▼
Becomes curious
        │
        ▼
Finds unusual behaviour
        │
        ▼
Discovers hidden clue
        │
        ▼
Attempts to decode puzzle
        │
        ▼
Finds another mystery
        │
        ▼
Returns later
        │
        ▼
Repeats
```

The project intentionally avoids providing a traditional "ending."

Instead, every solved mystery should naturally lead toward another.

---

# Feature Overview

The current planned feature set is summarized below.

| Feature | Status | Description |
|----------|--------|-------------|
| Global Countdown | Planned | One synchronized countdown shared worldwide. |
| Psychological Horror Experience | Planned | Suspense through uncertainty and atmosphere. |
| Hidden Pages | Planned | Secret routes discoverable only through investigation. |
| Puzzle Engine | Planned | Multi-layer cryptographic puzzle system. |
| Daily Evolution | Planned | Website changes over time without announcement. |
| Buy Time System | Planned | Visitors collectively influence the global countdown. |
| Decoder Reward System | Planned | First verified decoder receives a unique reward. |
| Premium Decoder Access | Planned | Temporary homepage message privileges for successful decoder. |
| DCoders Hall of Fame | Planned | Permanent historical record of verified decoders. |

---

> **Next Section:** **02 — System Architecture & Project Structure**
>
> This section defines the technical architecture, repository organization, frontend structure, backend responsibilities, component hierarchy and development philosophy.
---

# System Architecture

DCODE is designed as a modular, scalable web application where each subsystem has a clearly defined responsibility.

The project follows a **layered architecture**, allowing the frontend, backend, puzzle engine and administration tools to evolve independently without introducing unnecessary coupling.

At a high level, the system can be represented as follows.

```text
                        ┌─────────────────────┐
                        │     Visitor         │
                        └──────────┬──────────┘
                                   │
                                   ▼
                    ┌──────────────────────────┐
                    │      Frontend (UI)       │
                    │ HTML • CSS • JavaScript  │
                    └──────────┬───────────────┘
                               │
              ┌────────────────┼────────────────┐
              ▼                ▼                ▼
      Countdown Engine   Puzzle Engine    Visual Engine
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                     Backend Application Layer
                               │
          ┌────────────────────┼─────────────────────┐
          ▼                    ▼                     ▼
   Authentication        Payment System       Admin System
          │                    │                     │
          └────────────────────┼─────────────────────┘
                               ▼
                          Primary Database
                               │
                               ▼
                      Analytics & Event Logs
```

The frontend should never become responsible for business logic.

Its responsibility is presentation only.

The backend remains the single source of truth for every critical system.

---

# High-Level Components

| Component | Responsibility |
|------------|---------------|
| Frontend | User interface and interaction |
| Countdown Engine | Calculates and distributes the global countdown |
| Puzzle Engine | Controls puzzle progression and validation |
| Story Engine | Determines scheduled narrative changes |
| Payment Engine | Extends the global timer after successful payments |
| Decoder Verification | Confirms legitimate puzzle completion |
| Hall of Fame | Stores verified decoder records |
| Admin Dashboard | Internal moderation and management |
| Analytics | Collects anonymous usage statistics |

---

# Architecture Principles

The architecture follows several core principles.

| Principle | Description |
|-----------|-------------|
| Separation of Concerns | Each subsystem owns one responsibility. |
| Single Source of Truth | Countdown and puzzle states exist only on the backend. |
| Server Authority | Clients never determine official game state. |
| Scalability | Components should be independently expandable. |
| Security | Sensitive logic never resides in public code. |
| Modularity | Features should be replaceable without affecting unrelated systems. |

---

# Repository Structure

Current repository layout.

```text
DCODE/
│
├── assets/
│   ├── audio/
│   ├── fonts/
│   ├── icons/
│   ├── images/
│   └── videos/
│
├── css/
│   ├── animations.css
│   ├── components.css
│   ├── globals.css
│   ├── layout.css
│   └── themes.css
│
├── js/
│   ├── app.js
│   ├── countdown.js
│   ├── effects.js
│   ├── navigation.js
│   ├── puzzles.js
│   ├── utilities.js
│   └── ui.js
│
├── pages/
│   ├── archive/
│   ├── gateway/
│   ├── logs/
│   ├── signal/
│   ├── transmission/
│   └── hidden/
│
├── docs/
│
├── README.md
│
└── index.html
```

As development progresses, additional directories will be introduced for backend services, deployment scripts and operational tooling.

---

# Future Repository Layout

```text
DCODE/

frontend/

backend/

database/

payments/

authentication/

countdown/

puzzles/

analytics/

deployment/

admin/

documentation/

tests/

monitoring/
```

Each major system should remain isolated from unrelated components.

---

# Frontend Responsibilities

The frontend is responsible only for presentation.

It should never contain authoritative game logic.

Responsibilities include:

- Rendering pages
- Displaying the countdown
- Displaying clues
- Triggering animations
- User navigation
- Audio playback
- Theme switching
- Accessibility
- Responsive layouts

The frontend must never contain:

- Final puzzle solutions
- Decoder verification logic
- Secret encryption keys
- Administrative controls
- Payment verification
- Countdown authority

---

# Backend Responsibilities

The backend acts as the authoritative game server.

Responsibilities include:

- Maintaining the official countdown
- Synchronizing every connected client
- Validating payments
- Storing puzzle progress
- Scheduling story events
- Managing decoder verification
- Recording Hall of Fame entries
- Logging system events
- Admin authentication
- Rate limiting
- Anti-abuse controls

Every client should trust the backend—not other clients.

---

# Component Responsibilities

## Countdown Engine

Responsible for:

- Global countdown calculation
- Time synchronization
- Countdown extension
- Scheduled events
- Timer persistence

---

## Puzzle Engine

Responsible for:

- Puzzle activation
- Unlock conditions
- Hint scheduling
- Solution validation
- Progression logic

---

## Story Engine

Responsible for:

- Daily messages
- Environmental changes
- Story progression
- Event scheduling
- Timed reveals

---

## Payment Engine

Responsible for:

- Payment verification
- Timer extension
- Contribution history
- Fraud prevention
- Transaction logging

---

## Decoder Engine

Responsible for:

- Final solution validation
- Preventing duplicate claims
- Recording solve timestamps
- Granting temporary privileges
- Unlocking reward delivery

---

# Data Flow

The expected system flow is illustrated below.

```text
Visitor

↓

Loads Website

↓

Requests Countdown

↓

Backend Returns Official Countdown

↓

Visitor Explores

↓

Discovers Clues

↓

Attempts Puzzle

↓

Backend Validates

↓

If Incorrect

↓

Continue Investigation

↓

If Correct

↓

Unlock Next Stage
```

Every meaningful action should ultimately be verified by the backend.

---

# Client–Server Philosophy

The client should be considered untrusted.

Anything visible inside browser developer tools must be assumed discoverable.

Therefore:

✅ UI logic belongs in the browser.

❌ Secret logic does not.

Examples of client-side logic:

- Animations
- Theme changes
- Audio controls
- Visual glitches
- Menu interactions

Examples of server-side logic:

- Master puzzle verification
- Payment validation
- Countdown authority
- Decoder verification
- Reward unlocking

---

# Design Philosophy

DCODE should not feel like software.

It should feel like discovering something that was never intended to be found.

Every feature should answer one question before implementation:

> **"Does this increase curiosity without giving away certainty?"**

If the answer is **no**, the feature should be redesigned or removed.

---

> **Next Section:** **03 — Frontend Design System & User Experience**

This section defines the visual language, UI components, responsive design, interaction principles, atmosphere, animations and accessibility standards used throughout DCODE.
