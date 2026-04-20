# AI Landing Page Generator

An AI-powered web application that generates complete, ready-to-use landing pages from a simple product description. Fill out a short form about your product and get a full landing page you can copy or download instantly.

## Features

- **AI-Powered Generation** — Describe your product name, target audience, key benefits, and tone of voice to generate a tailored landing page
- **Two-Panel Layout** — Side-by-side form and live preview for a smooth generation experience
- **Copy & Download** — Export your generated landing page as clean HTML

## Tech Stack

- **Framework:** [Astro v6](https://astro.build/) (static site)
- **Styling:** Custom CSS design system with CSS custom properties
- **AI:** Claude API (Anthropic)
- **Languages:** Astro, CSS, JavaScript

## Getting Started

### Prerequisites

- Node.js v18+
- An [Anthropic API key](https://console.anthropic.com/)

### Installation

```bash
git clone https://github.com/madhumurthy16/ai-landing-page-generator.git
cd ai-landing-page-generator
npm install
```

### Run Locally

```bash
npm run dev
```

Open [http://localhost:4321](http://localhost:4321) in your browser.

## Commands

All commands are run from the root of the project:

| Command | Action |
| --- | --- |
| `npm install` | Install dependencies |
| `npm run dev` | Start dev server at `localhost:4321` |
| `npm run build` | Build production site to `./dist/` |
| `npm run preview` | Preview production build locally |

## Built with Claude Code

The hero section of this app was built using **[Claude Code](https://claude.ai/code)**, Anthropic's agentic coding tool. Claude Code was used to scaffold the component layout, implement the design system tokens, and iterate on the two-panel UI — dramatically accelerating the development process while keeping the code clean and maintainable.

A `CLAUDE.md` file is included at the root of the repo to provide Claude Code with project-specific context, architecture guidance, and dev commands whenever it's working in this codebase.
