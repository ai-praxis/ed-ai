# ed-ai: AI in Higher Education Research Hub

> A central repository for research, literature, and resources on AI interventions in higher education

## Overview

This repository serves as the **hub** for the AI-PRAXIS organization's research on artificial intelligence applications in higher education. It provides a centralized location for:

- Literature reviews and annotated bibliographies on AI in education
- Research notes and conceptual frameworks
- Funding strategies and grant opportunities
- Reusable templates and resources for research projects

## Philosophy

Rather than replacing existing educational infrastructure, we focus on **AI interventions that enhance and empower** current practices. Our approach emphasizes:

- Micro-interventions that support students and educators
- Ethical AI integration aligned with educational missions
- Institutional agency over AI tools and services
- Evidence-based design grounded in educational research

## Hub-and-Spoke Model

This repository follows a **hub-and-spoke architecture**:

- **Hub (this repo)**: General AI-in-education knowledge, literature, and resources
- **Spokes**: Project-specific repositories that build on hub foundations

### Current Spoke Projects

- `ed-ai-its`: Intelligent tutoring systems for language learning
- `ed-ai-session-prep`: AI-assisted preparation for tutoring sessions
- More to come...

Each spoke inherits the hub structure but adds project-specific work under `./project/`.

## Repository Structure

```
ed-ai/
├── research/
│   ├── literature/     # Literature reviews and bibliographies
│   ├── notes/          # Research notes and working documents
│   └── templates/      # Reusable research templates
├── funding/
│   ├── strategies/     # Funding planning and approaches
│   └── opportunities/  # Grant programs and funding sources
├── blog/               # Blog posts and reflections
├── logs/               # Project logs and updates
├── assets/             # Images, styles, and shared resources
└── _resources/         # Private working documents
```

## Getting Started

### Prerequisites

This project uses Nix flakes for reproducible development environments:

```bash
# Install Nix with flakes enabled
curl -L https://nixos.org/nix/install | sh

# Enable flakes (if needed)
mkdir -p ~/.config/nix
echo "experimental-features = nix-command flakes" >> ~/.config/nix/nix.conf
```

### Setup

```bash
# Clone the repository
git clone https://github.com/ai-praxis/ed-ai.git
cd ed-ai

# Enter the development environment (using direnv)
direnv allow

# Or manually activate the Nix shell
nix develop
```

### Building the Website

This repository uses Quarto for documentation:

```bash
# Preview the website locally
quarto preview

# Build the static site
quarto render
```

## Contributing

We welcome collaboration from researchers, educators, and practitioners interested in ethical AI applications in higher education. Please see individual spoke repositories for project-specific contribution guidelines.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For inquiries about collaboration or the AI-PRAXIS organization, please open an issue or reach out through the organization's GitHub page.
