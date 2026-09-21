```ruby
███████╗██╗███████╗███╗   ███╗
██╔════╝██║██╔════╝████╗ ████║
███████╗██║█████╗  ██╔████╔██║
╚════██║██║██╔══╝  ██║╚██╔╝██║
███████║██║███████╗██║ ╚═╝ ██║
╚══════╝╚═╝╚══════╝╚═╝     ╚═╝
```

**Muhammad Balal Ansar(Cyber Security Expert)**

[![Cybersecurity Projects](https://img.shields.io/badge/Cybersecurity--Projects-Project%20%231



> Full-stack SIEM dashboard with real-time log correlation and MITRE ATT&CK attack scenario simulation engine.

*This is a quick overview — security theory, architecture, and full walkthroughs are in the [learn modules](#learn).*


**[Screenshots & live demo →](DEMO.md)**

## What It Does

- Real-time log ingestion and event correlation with three rule types (Threshold, Sequence, Aggregation)
- Four YAML-based attack playbooks mapped to MITRE ATT&CK (brute force, DNS tunneling, phishing, privilege escalation)
- Server-Sent Events for live alert feed with paginated, filterable log viewer
- Alert lifecycle management (acknowledge, investigate, resolve, false positive)
- Attack simulation engine that generates realistic multi-stage security events
- Built with Just for task automation with full Docker Compose deployment

## Quick Start

```bash

docker compose up -d
```

Visit `http://localhost:8431` or the live demo at [siem.carterperez-dev.com](https://siem.carterperez-dev.com/)

> [!TIP]
> This project uses [`just`](https://github.com/casey/just) as a command runner. Type `just` to see all available commands.
> Install: `curl -sSf https://just.systems/install.sh | bash -s -- --to ~/.local/bin`

## Stack

**Backend:** Flask, MongoEngine, Redis Streams, Pydantic, Argon2, JWT, Gunicorn

**Frontend:** React 19, TypeScript, Vite, TanStack Query, Zustand, visx, SCSS Modules

**Data:** MongoDB 8, Redis 7
## Learn

This project includes step-by-step learning materials covering security theory, architecture, and implementation.

| Module | Topic |
|--------|-------|
| [00 - Overview](learn/00-OVERVIEW.md) | Prerequisites and quick start |
| [01 - Concepts](learn/01-CONCEPTS.md) | Security theory and real-world breaches |
| [02 - Architecture](learn/02-ARCHITECTURE.md) | System design and data flow |
| [03 - Implementation](learn/03-IMPLEMENTATION.md) | Code walkthrough |
| [04 - Challenges](learn/04-CHALLENGES.md) | Extension ideas and exercises |

## License

AGPL 3.0
