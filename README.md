# Mermaid Visual Charts

Generate clean, structured visual diagrams from natural language descriptions or bullet-point notes. Primary use cases: RACI swimlane diagrams, MECE issue trees, decision trees, and process flows.

## Tech Stack

- **CLI Tool:** Mermaid CLI (@mermaid-js/mermaid-cli)
- **Backend:** Node.js
- **Output Formats:** SVG, PNG
- **Deployment:** N/A

## Getting Started

### Prerequisites

- Node.js 18+
- npm

### Installation

Install Mermaid CLI globally:

```bash
npm install -g @mermaid-js/mermaid-cli
```

Verify installation:

```bash
mmdc --version
```

### Usage

Generate diagrams using the Mermaid CLI:

```bash
# Generate SVG output
mmdc -i input.mmd -o output.svg

# Generate PNG output
mmdc -i input.mmd -o output.png
```

## Project Structure

```
mermaid-visual-charts/
├── examples/         # Example Mermaid diagrams
├── output/           # Generated diagrams (SVG/PNG)
├── .gitignore        # Git ignore rules
├── package.json      # Dependencies
├── Briefing          # Project requirements
└── README.md         # This file
```

## Features

- Generate RACI swimlane diagrams showing cross-functional handoffs
- Create MECE-structured issue trees (McKinsey/Minto style)
- Build decision trees with binary or multi-path flows
- Visualize sequential process workflows with decision points
- Automatic validation for structural issues (MECE violations, circular dependencies, orphaned nodes)
- Clean, production-ready output suitable for executive presentations

## Diagram Types

1. **Swimlane/RACI flows**: Show cross-functional handoffs with role accountability
2. **Issue trees**: MECE-structured problem decomposition
3. **Decision trees**: Binary or multi-path decision flows
4. **Process flows**: Sequential workflows with decision points

## Validation Layer

The system checks for structural issues before rendering:
- MECE violations (overlapping or missing branches)
- Undefined handoffs in process flows
- Circular dependencies
- Orphaned nodes

## System Behavior

When provided with input:
1. Parse structure and intent
2. Generate Mermaid syntax
3. Flag any structural issues detected
4. Render diagram
5. Confirm output location

## License

MIT

---

**Created:** November 2025
**Last Updated:** November 2025
