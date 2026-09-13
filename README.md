# NYX

### Local-First AI Desktop Agent for Windows

<p align="center">
  <img src="assets/NYX-mark.svg" alt="NYX Logo" width="180">
</p>

<h1 align="center">NYX</h1>

<p align="center">
  <strong>Local-First AI Desktop Agent for Windows</strong>
</p>

<p align="center">
  A personal AI system designed to understand, reason, see, speak, analyze, code, and interact with a Windows computer.
</p>

**Status:** 🚧 Active Development  
**Platform:** Windows  
**Architecture:** Local-first, multi-model AI agent  
**Source:** Private

---

## 🌙 What is NYX?

NYX is a personal AI desktop agent I'm developing to explore what happens when a local AI is deeply integrated with a computer instead of existing only inside a chat window.

The goal is to create one intelligent system capable of combining conversation, reasoning, computer vision, coding, research, data analysis, memory, and desktop interaction.

Instead of treating every request as an isolated command, NYX is being designed to understand the user's goal, determine which capabilities are needed, perform the work, observe the results, recover from failures, and verify that the original goal was actually completed.

NYX runs primarily on local AI models and is designed around privacy, user control, transparency, and safe computer interaction.

---

# ✨ Core Capabilities

| Capability                     | Description                                                                                                                     |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| 🗣️ **Voice Interaction**       | Continuous local speech recognition, natural speech generation, interruption, wake-word support, and conversational turn-taking |
| 🖥️ **Desktop Interaction**     | Works with Windows applications, windows, files, folders, and supported UI elements                                             |
| 👁️ **Computer Vision**         | Understands screenshots and visual information using local vision models                                                        |
| 🧠 **Local AI**                | Uses multiple locally hosted AI models for conversation, reasoning, coding, and vision                                          |
| 💻 **Coding Assistant**        | Can understand projects, inspect source files, help debug code, review projects, and assist with development workflows          |
| 🌐 **Browser & Research**      | Browser automation, web research, information retrieval, and source-aware research workflows                                    |
| 📊 **Data Intelligence**       | Designed to analyze datasets, calculate statistics, discover patterns, compare information, and visualize results               |
| 🧩 **Task Planning**           | Breaks complex requests into multiple capabilities and execution steps                                                          |
| 🧠 **Memory & Context**        | Maintains local conversation context, preferences, knowledge, and persistent memories                                           |
| 📁 **Workspace Awareness**     | Understands active projects, applications, files, and development workspaces                                                    |
| 🔐 **Safety & Permissions**    | Confirmation gates, capability permissions, interruption controls, and safeguards around sensitive actions                      |
| 🔄 **Recovery & Verification** | Designed to detect failures, replan tasks, verify results, and avoid falsely claiming completion                                |

---

# 🖼️ NYX Interface

NYX has a custom desktop interface built around the idea that the user should be able to see what the AI is doing.

The interface includes areas for:

- Conversation
- Current tasks
- Activity history
- System health
- Memory
- Permissions
- Connected devices
- Analysis
- Simulations
- Notifications
- Workspace tools
- AI capabilities

NYX can also operate as a small ambient desktop presence and expand into a larger workspace when more detailed interaction is needed.

## Screenshots

> Screenshots of the NYX interface will be added here.

<!-- Example:
![NYX Desktop](screenshots/nyx-desktop.png)
-->

---

# 🌍 NYX World

**NYX World** is an integrated globe and public-data workspace built directly into NYX.

It expands the assistant beyond traditional chat by giving NYX a visual environment for exploring geographic and real-world information.

The workspace is designed to support interactive geographic data, public datasets, environmental information, transportation information, and other world-oriented analysis.

NYX World is part of a larger goal: allowing the assistant to **show information visually instead of only describing it through text.**

## NYX World Preview

> Screenshot coming soon.

<!-- Example:
![NYX World](screenshots/nyx-world.png)
-->

---

# 🧠 How NYX Works

NYX is more than a language model connected directly to a collection of commands.

The system separates conversation, context, planning, execution, observation, and verification.

```text
                    USER
                      │
                      ▼
             Request Understanding
                      │
                      ▼
              Context Resolution
                      │
                      ▼
              Goal Decomposition
                      │
                      ▼
           Capability Composition
                      │
                      ▼
                  Planning
                      │
                      ▼
             Permission Checks
                      │
                      ▼
                  Execution
                      │
                      ▼
                 Observation
                      │
                      ▼
            Verification / Recovery
                      │
                      ▼
                   RESPONSE

This architecture allows a single request to involve several systems.

For example:

"Look at the chart on monitor 2 and analyze the trend."

            │
            ▼

Screen Awareness
      +
Computer Vision
      +
Market/Data Tools
      +
Data Analysis
      +
Visualization
      +
Response

The goal is not simply to execute a tool.

The goal is to complete the user's actual objective.

🤖 Local AI Model Stack

NYX uses specialized local models for different workloads.

Model	Role
Qwen3 14B	Primary conversation and reasoning
Qwen3 8B	Faster fallback model
Qwen2.5 Coder 7B	Programming and software development
LLaVA	Screen and image understanding
Faster-Whisper	Speech recognition
Piper	Local speech generation

Models are hosted locally through Ollama and supporting local runtimes.

Using multiple models allows NYX to choose a model appropriate for the task instead of forcing every workload through one system.

🗣️ Voice System

Voice is a major part of NYX.

The system is being designed for conversational interaction rather than traditional command-and-response voice control.

Current architecture includes:

Local speech recognition
Voice activity detection
Wake-word support
Local text-to-speech
Progressive spoken responses
Conversation interruption
Speaker recognition
Microphone and speaker selection
Conversation-state management
Pronunciation preferences
Response-style preferences

NYX is designed so that speaking and listening remain interruptible.

If the user begins speaking while NYX is responding, the system can stop and return control to the user.

👁️ Vision & Screen Understanding

NYX can use visual information from the computer as another source of context.

The vision architecture combines several forms of information where available:

Application State
        +
Window Information
        +
UI / Accessibility Data
        +
Screen Capture
        +
Vision Model
        │
        ▼
Structured Screen Understanding

This allows NYX to reason about what the user is currently working on instead of relying entirely on text descriptions.

A major development goal is ensuring that visual claims are always grounded in actual screen evidence.

💻 Software Development

NYX also acts as a local software-development assistant.

The coding system is designed to work with real development projects rather than only generate isolated code snippets.

Capabilities include:

Project inspection
Source-code search
File reading
Code explanation
Debugging assistance
Code review
Multi-file reasoning
Dependency analysis
Development workspace awareness
Test discovery
Static-analysis integration
Transactional code changes
Verification before completion claims

NYX integrates with development tools including Visual Studio Code and Git.

The long-term goal is for NYX to behave more like a development teammate than a code generator.

📊 Data Intelligence

NYX is being expanded with a general-purpose data-analysis system.

The goal is to allow requests such as:

"Analyze this dataset and show me anything unusual."

"Compare these companies."

"Find patterns in this chart."

"Show me what changed."

The analysis architecture is being designed around actual computation rather than asking the language model to perform large calculations mentally.

Planned and developing capabilities include:

Data ingestion
Cleaning and normalization
Statistical analysis
Time-series analysis
Pattern detection
Anomaly detection
Comparison analysis
Hypothesis testing
Interactive charts
Reproducible analysis
Evidence-backed conclusions
🧠 Memory & Context

NYX maintains local context to make interactions more continuous.

The memory system is designed around:

Conversation history
User preferences
Knowledge
Task history
Research
Context retrieval
Semantic similarity
Provenance
Information freshness

An important architectural principle is context isolation.

Screen information, project information, research results, memories, and other sources are kept logically separated so unrelated information does not accidentally influence the wrong task.

🛠️ Technology

NYX is built using a combination of AI, desktop, browser, voice, and development technologies.

Core
Python
PySide6
Qt / QML
SQLite
Git
AI
Ollama
Qwen
LLaVA
PyTorch
Transformers
ONNX Runtime
Voice
Faster-Whisper
Piper
Silero VAD
openWakeWord
SpeechBrain
Desktop
Windows UI Automation
PyWin32
pywinauto
Windows accessibility interfaces
Browser
Playwright
Chromium / Chrome automation
Web research tooling
Development
Visual Studio Code
GitHub
Ruff
automated testing
security and dependency analysis
🔐 Local-First Design

Privacy is one of the core design principles behind NYX.

Whenever practical, processing occurs locally on the computer.

Local components include:

AI inference
Speech recognition
Speech generation
Memory
Conversation history
Screen understanding
Coding assistance
Desktop automation

Network-dependent capabilities such as current web research are treated separately from the local runtime.

🛡️ Safety

Giving an AI access to a computer requires stronger safeguards than a normal chatbot.

NYX therefore includes concepts such as:

Capability permissions
Confirmation for sensitive actions
Application restrictions
File-access boundaries
Screen-capture controls
User interruption
Emergency stopping
Task cancellation
Action history
Failure recovery
Transactional changes
Backup and rollback
Goal verification

The system is designed around the principle that being able to perform an action does not automatically mean NYX should perform it without permission.

🔄 Reliability Engineering

One of the biggest areas of development is agent reliability.

NYX is being designed to handle problems such as:

Misunderstood requests
Incorrect context
Wrong tool selection
Invalid tool arguments
Stale observations
Partial task completion
Failed actions
User corrections
Interruptions
Application changes during a task
Model failures
Network failures
Recovery after restart

Real-world failures discovered while using NYX are converted into regression tests.

This creates a growing behavioral test suite based on actual interactions rather than only synthetic examples.

🧪 Development Philosophy

NYX follows several important design principles:

One NYX, many capabilities

Features should behave like abilities belonging to one assistant rather than disconnected applications.

Conversation comes first

Normal conversation should remain natural and should not be forced through a tool system unnecessarily.

Understand before acting

The system should resolve what the user actually means before selecting tools.

Observe before claiming

NYX should never claim something happened simply because a command was issued.

Verify the goal

A successful tool call does not necessarily mean the user's request was completed.

Recover intelligently

When something fails, NYX should understand the failure and determine whether another safe approach is available.

Keep the user informed

Long-running tasks should expose understandable progress without exposing private internal reasoning.

🚧 Current Development

NYX is under active development.

Current work is focused heavily on improving the agent architecture, including:

Context isolation
Request understanding
Referential follow-ups
Multi-capability planning
Tool argument validation
Screen grounding
Workspace grounding
Observation freshness
Failure recovery
Replanning
Goal verification
Long-running task reliability
User-visible activity reporting

The current priority is reliability over simply adding more tools.

🎥 Demonstrations

This repository will eventually include demonstrations of:

Voice Interaction

Demo coming soon.

Desktop Control

Demo coming soon.

Computer Vision

Demo coming soon.

Coding

Demo coming soon.

Data Analysis

Demo coming soon.

NYX World

Demo coming soon.

🗺️ Future Direction

NYX is ultimately intended to become a general-purpose local AI environment capable of combining:

Conversation
     +
Reasoning
     +
Vision
     +
Voice
     +
Coding
     +
Research
     +
Data Intelligence
     +
Computer Interaction
     +
Long-Term Context

Rather than building a separate AI application for every task, the goal is to allow one assistant to dynamically combine the capabilities required for the user's objective.

📸 Showcase Repository

This repository contains the public showcase for NYX.

It will contain:

Screenshots
Demonstrations
Architecture explanations
Feature descriptions
Development updates
Public documentation

The production NYX source repository is private.

Personal configuration, credentials, memory databases, model files, runtime logs, private data, and production source code are not included in this repository.

👨‍💻 Creator

Keron Antoine

NYX is an independently developed personal AI project exploring local AI, agent architecture, human-computer interaction, computer vision, voice interfaces, automation, and intelligent desktop systems.

⭐ NYX

One assistant. Many capabilities. Local first.
```
