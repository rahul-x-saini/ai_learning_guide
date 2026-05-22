# AI Guide Generator (CrewAI Multi-Agent System)

## Overview
This project is a multi-agent AI system built using CrewAI that automatically generates beginner-friendly “Getting Started” guides from raw learning resources.

It uses a two-stage pipeline:
1. **Research Crew (Hierarchical)** – Collects and compiles detailed information from multiple sources such as YouTube, web pages, research papers, and documents.
2. **Writing Crew (Sequential)** – Transforms the research into a structured, beginner-friendly guide and refines it for clarity and completeness.

## How It Works
- Users provide optional input sources (links, documents, etc.).
- The **Research Crew** uses specialized agents (YouTube, Web, Arxiv, Document) managed by a coordinator to generate a comprehensive research report.
- The **Writing Crew** converts this report into a step-by-step guide and polishes it for beginners.
- The entire process is orchestrated using a **CrewAI Flow** with state management.

## Key Features
- Multi-agent architecture with role-based specialization
- Hierarchical + sequential workflow design
- Automated research aggregation from multiple source types
- Beginner-friendly documentation generation
- End-to-end pipeline orchestration using CrewAI Flow


## Usage
Run the main flow:
```bash
crewai flow kickoff
