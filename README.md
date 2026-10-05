# Stage 2026 — Mohamed Omezzine

Portfolio and technical documentation from the 2026 summer internship at **CyberShield TN**.

## Main subject

**Automatisation du traitement des tickets et des appels entrants par l'intelligence artificielle**

The work covers a security-operations support pipeline that combines ticketing, human-approved AI assistance, Telegram notifications, and real-time voice support.

## Repository contents

| Document | Focus |
|---|---|
| `Rapport Mohamed omezzine.pdf` | Full internship report: context, architecture, implementation, testing, and lessons learned |
| `Documentation_Workflow_SOC_Telegram.docx` | Telegram workflow improvements, ticket correlation, agent validation, retry loop, and multi-worker state |
| `Migration n8n Mohamed Omezzine.docx` | Migration from a single n8n instance to queue mode with Redis and three workers |
| `annexe Workflows.pdf` | Telegram/Ollama workflow diagrams and 3CX voice workflow diagram |
| `Annexe source code.pdf` | Technical source-code and AudioSocket/Docker annexes |
| `docker.docx` | Docker and Docker Compose command reference |
| `uml.docx` | UML/design annex |

## Technical highlights

- n8n workflow orchestration in queue mode with **Redis** and three workers.
- Human-in-the-loop validation before an AI-generated ticket response is sent.
- Telegram ticket notification, agent availability resolution, anti-double-assignment locking, and retry polling.
- Zammad ticketing integrated with **Ollama** for local AI assistance.
- 3CX/Asterisk integration through **AudioSocket** and a Python bridge.
- Real-time speech pipeline with **faster-whisper** and **edge-tts**.
- Docker-based development and distributed troubleshooting across WSL2, VMs, and network tunnels.

## Privacy note

This repository is a public portfolio of academic and internship documentation. The daily activity-report PDF was intentionally removed. A credential scan found no passwords, API keys, bearer tokens, bot tokens, private keys, or n8n encryption keys in the remaining documents.
