# 🧬 Molecular Canvas

<div align="center">

![Molecular Canvas Banner](./assets/branding/banner.png)

**An interactive AI-powered molecular visualization, chemistry simulation, and education platform.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![Build Status](https://github.com/your-org/molecular-canvas/actions/workflows/ci.yml/badge.svg)](https://github.com/your-org/molecular-canvas/actions)
[![codecov](https://codecov.io/gh/your-org/molecular-canvas/branch/main/graph/badge.svg)](https://codecov.io/gh/your-org/molecular-canvas)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./docs/Contributing.md)
[![Discord](https://img.shields.io/discord/your-server-id?label=Discord&logo=discord)](https://discord.gg/your-invite)

[🚀 Live Demo](https://molecular-canvas.app) · [📖 Documentation](./docs/) · [🐛 Report Bug](https://github.com/your-org/molecular-canvas/issues/new?template=bug_report.md) · [💡 Request Feature](https://github.com/your-org/molecular-canvas/issues/new?template=feature_request.md)

</div>

---

## ✨ What is Molecular Canvas?

Molecular Canvas is a next-generation, open-source platform for molecular visualization, chemistry simulation, and AI-guided science education. It bridges the gap between professional cheminformatics tools and accessible, interactive learning environments.

Whether you are a student learning bonding for the first time, a researcher visualizing protein folding, or an educator building interactive chemistry lessons — Molecular Canvas is built for you.

---

## 🌟 Key Features

| Feature | Status |
|---|---|
| 🔬 Interactive Molecule Builder | 🚧 In Development |
| ⚛️ Electron Orbital Visualization | 🚧 In Development |
| 🧪 Chemical Reaction Simulator | 📋 Planned |
| 🤖 AI Chemistry Tutor | 📋 Planned |
| 🧫 Protein & Biomolecule Viewer | 📋 Planned |
| 📊 Molecular Dynamics Engine | 📋 Planned |
| 🌐 Collaborative Editing | 🔮 Future |
| 🥽 VR/AR Molecular Exploration | 🔮 Future |

> See [Features.md](./docs/Features.md) and [Roadmap.md](./docs/Roadmap.md) for full details.

---

## 🏗️ Architecture Overview

```
┌─────────────────────────────────────────────────────────┐
│                   Molecular Canvas                       │
├──────────────┬──────────────┬───────────────────────────┤
│   Frontend   │   Backend    │      AI Service            │
│  React + R3F │  Node/Express│  Python FastAPI + Models  │
├──────────────┴──────────────┴───────────────────────────┤
│              Molecular Engine (Core)                     │
│     Atoms · Bonds · Geometry · Reaction Engine          │
├─────────────────────────────────────────────────────────┤
│              Rendering Engine (WebGL/Three.js)           │
│     Materials · Shaders · Particles · Post-FX           │
├─────────────────────────────────────────────────────────┤
│              Physics Engine                              │
│     Force Fields · MD Simulation · Energy Calc          │
└─────────────────────────────────────────────────────────┘
```

> See [Architecture.md](./docs/Architecture.md) for the full system design.

---

## 🚀 Quick Start

### Prerequisites

- Node.js >= 18.x
- Python >= 3.10
- Docker & Docker Compose (optional but recommended)
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/molecular-canvas.git
cd molecular-canvas
```

### 2. Setup Environment Variables

```bash
cp .env.example .env
# Edit .env with your configuration
```

### 3. Install Dependencies

```bash
# Frontend
cd frontend && npm install

# Backend
cd ../backend && npm install

# AI Service
cd ../ai-service && pip install -r requirements.txt
```

### 4. Start Development Servers

```bash
# From root — starts all services
docker-compose up -d

# Or manually:
cd frontend && npm run dev
cd backend && npm run dev
cd ai-service && uvicorn main:app --reload
```

### 5. Open in Browser

Visit `http://localhost:3000` to see Molecular Canvas running locally.

---

## 📂 Project Structure

```
molecular-canvas/
├── frontend/          # React + Three.js web application
├── backend/           # Node.js + Express REST API
├── ai-service/        # Python FastAPI AI microservice
├── molecular-engine/  # Core chemistry logic (shared)
├── rendering-engine/  # WebGL / Three.js rendering pipeline
├── physics-engine/    # Molecular dynamics & force fields
├── database/          # DB schemas, migrations, seeds
├── assets/            # Static assets, models, textures
├── docs/              # All project documentation
├── tests/             # Integration & E2E tests
├── devops/            # Docker, CI/CD, deployment scripts
└── .github/           # GitHub Actions, templates
```

> See [FolderStructure.md](./docs/FolderStructure.md) for the complete annotated tree.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend Framework | React 18, TypeScript |
| 3D Rendering | Three.js, React Three Fiber |
| Shaders | GLSL, WebGL2 |
| State Management | Zustand / Jotai |
| Backend | Node.js, Express, TypeScript |
| AI Service | Python, FastAPI, PyTorch |
| Chemistry Libraries | RDKit, OpenBabel |
| Database | PostgreSQL, Redis |
| Authentication | JWT, OAuth 2.0 |
| Deployment | Docker, Kubernetes |
| CI/CD | GitHub Actions |

> See [TechStack.md](./docs/TechStack.md) for the full rationale.

---

## 📖 Documentation

| Document | Description |
|---|---|
| [Vision.md](./docs/Vision.md) | Long-term project vision |
| [Architecture.md](./docs/Architecture.md) | System architecture |
| [Roadmap.md](./docs/Roadmap.md) | Development roadmap & milestones |
| [Features.md](./docs/Features.md) | Feature list & specs |
| [API.md](./docs/API.md) | REST & WebSocket API reference |
| [DevelopmentGuide.md](./docs/DevelopmentGuide.md) | Dev setup & workflow |
| [Contributing.md](./docs/Contributing.md) | Contribution guidelines |
| [TechStack.md](./docs/TechStack.md) | Technology choices |
| [CodingStandards.md](./docs/CodingStandards.md) | Code style guide |
| [TestingStrategy.md](./docs/TestingStrategy.md) | Testing approach |
| [Deployment.md](./docs/Deployment.md) | Deployment instructions |
| [Security.md](./docs/Security.md) | Security policies |
| [Glossary.md](./docs/Glossary.md) | Domain terminology |

---

## 🤝 Contributing

We welcome contributions of all kinds! Please read our [Contributing Guide](./docs/Contributing.md) before opening a PR.

- 🐛 [Report a bug](https://github.com/your-org/molecular-canvas/issues/new?template=bug_report.md)
- 💡 [Suggest a feature](https://github.com/your-org/molecular-canvas/issues/new?template=feature_request.md)
- 📖 [Improve documentation](./docs/)
- 🔬 [Contribute chemistry logic](./molecular-engine/)

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

---

## 🙏 Acknowledgements

- [Three.js](https://threejs.org/) for the incredible 3D library
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber) for React-native 3D
- [RDKit](https://www.rdkit.org/) for cheminformatics
- [OpenBabel](https://openbabel.org/) for chemical file format support
- The entire open chemistry community

---

<div align="center">
Made with ❤️ for scientists, students, and curious minds everywhere.

⭐ Star this repo if you find it useful!
</div>
