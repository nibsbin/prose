# Prose

This is a framework I use for vibe coding.

## Core Philosophy

**Coding** is the art of communicating instructions to machines--so it makes sense that that LLMs can translate English into code better than me. After all, [the transformer](https://arxiv.org/pdf/1706.03762)--the cornerstone component in large language model (LLM) architecture that enables long-range pattern recognition--was originally created for translation tasks. Translating English to code is probably easier than translating English to French.

**Programming** is the art of building your ideas into virtual systems. Programming demands innotative ideas, good taste, and the ability to adapt to new contexts that lie outside of the distribution of an LLM's training data. I don't expect LLM-based AI agents to be better at programming than me in the near-term. LLMs can abstract ideas, think logically, and translate robustly--but my neural network (i.e., brain) is equipped for the complex problems posed by natural selection. Its architecture has been tuned by a stochastic algorithm that has sustained life for billions of years and created intelligence from nothing. I will continue to add creative and computational value as a high-level programmer. Probably.

The Prose framework facillitates my role as the high-level programmer by helping me:
- Express my ideas, taste, and context to the agent
- Validate and tweak the agent's trajectory
- Maintain awareness of my project's evolving concepts and codebase
- Iterate faster

Prose is not dogmatic; tailor it for your own style and use cases. Here's a starting point:

## The Structure

Prose involves two types of markdown documents:

- **Designs** are authoritative over the project's desired state. They capture my ideas and intent through medium to high-level specifications.
- **Plans** describe actionable phases that take the project from its current state to the desired state.

And uses two types of agents:

- **Architect** drafts design documents and plans based on your high-level intent and specifications.
- **Programmer** implements plans in your codebase.

A fresh Prose project set up for [GitHub Copilot coding agent](https://docs.github.com/en/copilot/concepts/agents/coding-agent/about-coding-agent) would have the following structure to accomodate these files:

```bash
.
├── .github
│   └── agents
│       ├── architect.yml
│       └── programmer.yml
├── prose/
│   ├── designs/
│   └── plans/
```

## High-level Workflow

Express and implement your ideas with the following steps:

1. Submit a new task to GitHub Copilot using the Architect agent.    
2. The Architect:
    - Edits design document in `prose/designs/` to captures your intent.
    - Drafts a plan document in `prose/plans/` that outlines actionable phases to implement the design.
3. Review the design and plan documents to align them with your vision and maintain awareness over your project.
4. Submit a new task to implement the plan using the Programmer agent.
5. Review the summary of changes reported by the Programmer agent.

## Example
