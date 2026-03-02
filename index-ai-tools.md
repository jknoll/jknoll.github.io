---
title: AI Tools Portfolio
layout: default
author: Justin F. Knoll
profile_image: profile-400.jpg
---

<style>
/* Layout - narrower max-width for readable line length */
.wrapper {
  max-width: 780px !important;
  padding-right: 30px !important;
  padding-left: 30px !important;
}
.page-content {
  padding-left: 220px;
}

/* Icon formatting */
.cert-icon { width: 16px; height: 16px; vertical-align: middle; margin-right: 4px; }
.issuer-cell { white-space: nowrap; }

/* Profile spacing */
.profile-section { margin-bottom: 30px; }

/* AI tools line */
.ai-tools { color: #586069; font-size: 0.92em; margin-top: 4px; }
.ai-tools strong { color: #24292e; }

/* Table of contents */
.toc-sidebar {
  position: fixed;
  left: 20px;
  top: 100px;
  width: 180px;
  font-size: 0.85em;
  background: #f8f8f8;
  padding: 15px;
  border-radius: 8px;
}
.toc-sidebar ul { list-style: none; padding: 0; margin: 0; }
.toc-sidebar li { margin-bottom: 8px; }
.toc-sidebar a { color: #666; text-decoration: none; }
.toc-sidebar a:hover { color: #0366d6; }
.toc-sidebar .toc-h2 { font-weight: 600; margin-top: 10px; }
.toc-sidebar .toc-h3 { padding-left: 10px; font-size: 0.9em; }

@media (max-width: 600px) {
  .toc-sidebar { display: none; }
  .page-content { padding-left: 0; }
}
</style>

<nav class="toc-sidebar">
<ul>
<li class="toc-h2"><a href="#introduction">Introduction</a></li>
<li class="toc-h2"><a href="#ai-applications">Applications</a></li>
<li class="toc-h2"><a href="#aiml-research">Research</a></li>
<li class="toc-h2"><a href="#ai-agents--visualization">Agents</a></li>
<li class="toc-h2"><a href="#hackathon-projects">Hackathons</a></li>
<li class="toc-h2"><a href="#claude-code-developer-tools">Dev Tools</a></li>
<li class="toc-h2"><a href="#ai-tools-summary">Tools Summary</a></li>
</ul>
</nav>

<div class="profile-section">
  <img src="{{ page.profile_image }}" alt="Profile Photo" class="profile-photo" style="width: 200px; height: 200px; border-radius: 50%; object-fit: cover;">
</div>

# Introduction

This page catalogs all projects built with [Claude Code](https://claude.ai/code) and the broader set of AI tools used in their production. Across these projects, I've used large language models, video and image generation APIs, vision transformers, agent orchestration frameworks, speech models, 3D modeling tools, and distributed training infrastructure.

## AI Applications

### [Clinical Trial Compass](https://github.com/jknoll/clinical-trial-copilot)
*February 2026*

AI-powered clinical trial navigator for patients and caregivers. Uses multi-agent orchestration to conduct patient interviews, search ClinicalTrials.gov, score eligibility against inclusion/exclusion criteria, and generate plain-language reports with interactive visualizations. Built for the "Built with Opus 4.6" Hackathon (Cerebral Valley x Anthropic, Feb 2026). Includes a companion iOS HealthKit app ([clinical-trial-health-ios](https://github.com/jknoll/clinical-trial-health-ios)) for real-time health data integration.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Opus 4.6 · Claude Sonnet 4.5 · Claude Haiku 4.5 · Anthropic API (tool use) · Claude Code</p>

### [AdFlow: Agentic Creative Director](https://github.com/jknoll/adflow)
*January 2026*

Automatically generates video advertisements from product URLs. Extracts product metadata via web scraping (JSON-LD, Open Graph, HTML parsing), uses multi-agent workflows to craft ad scripts and video prompts, and generates short video ads via multiple providers. Features dual Web UI and CLI interfaces, real-time progress tracking, and a REST API.

Submitted to the Agentic Orchestration Hack hosted by CreatorsCorner and AWS Builder Loft in San Francisco.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Agent SDK · Veo 3 Fast (Kie.ai) · Veo 3 Quality (Kie.ai) · WAN 2.6 720p/1080p (FreePik) · TinyFish / Mino AI · Claude Code</p>

### [Fakecation](https://github.com/jknoll/photo-app)
*February 2026*

AI-powered vacation photo compositing app. Upload a photo and choose a famous landmark destination; the app composites your image into the scene with photorealistic lighting and perspective. Includes same-day printing at 8,000+ Walgreens locations via the Walgreens Photo Prints API.

<p class="ai-tools"><strong>AI Tools:</strong> Nano Banana Pro / Gemini 3 Pro Image (Kie.ai) · Cloudinary · Claude Code</p>

### [Accessible Now](https://github.com/jknoll/accessible-now)
*2025*

Web accessibility proxy that transforms any URL into genuinely accessible HTML. Paste a URL, and the system uses vision models to analyze the page layout and content, then reasoning models to restructure it for screen readers and assistive technology.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Sonnet 4.5 (vision) · Claude Opus 4.6 (reasoning) · Claude Code</p>

### [Claude Strudel](https://github.com/jknoll/claude-strudel)
*2025*

AI-powered music composition interface combining Claude with Strudel.js live coding. Describe music in natural language and Claude generates Strudel patterns that play in the browser in real time.

<p class="ai-tools"><strong>AI Tools:</strong> Claude API · Strudel.js · Claude Code</p>

## AI/ML Research

### [FungiTastic Hierarchical Classifier](https://github.com/jknoll/amanita) ($5K Grant Recipient)
*January 2026*

Modified BEiT vision transformer (87.9M parameters) for hierarchical, multi-task taxonomic classification of fungi across six biological ranks. Trained on the FungiTastic dataset (~350K observations, >600K images, >5K species) with weighted cross-entropy loss. Achieved 89.91% top-1 accuracy at phylum level and 45.43% at species level. Includes analysis of dangerous species like *Amanita phalloides* (death cap). Supported by a $5K GPU credit research grant from Strong Compute.

<p class="ai-tools"><strong>AI Tools:</strong> BEiT Vision Transformer · Strong Compute ISC (GPU cluster) · Weights & Biases · Claude Code</p>

### [Chess Theme and Opening Multilabel Classifier](https://github.com/jknoll/chess-theme-classifier) (Grant Recipient)
*April 2025–July 2025*

Deep CNN for multi-label classification of chess positions from the lichess puzzles dataset. 1,616 labels across themes (back rank mate, zugzwang, etc.) and openings (Sicilian Defense, English Opening, etc.). Best F1: 0.99 on ~5M training samples.

<p class="ai-tools"><strong>AI Tools:</strong> PyTorch CNN · Weights & Biases · TensorBoard · Claude Code</p>

### Chess AI Hackathon Series (Six-Time Winner)
*August 2024–March 2025*

Deep learning chess engine trained on a 72xA100 GPU cluster. Explored CNN, dilated convolution, ResNet, transformer, and multi-head self-attention architectures. Inspired by Adam Karvonen's research on emergent world models in chess-playing language models. Won 6 of 7 tournament instances, earning $10K+ in GPU compute credits. Sponsored by Strong Compute (YC W22).

<p class="ai-tools"><strong>AI Tools:</strong> PyTorch (CNN / ResNet / Transformer) · Strong Compute (72xA100) · Claude Code</p>

### [QuantumBench](https://github.com/jknoll/quantumbench)
*2025*

Quantum computing fine-tune dataset generator. Creates prompt-completion pairs for Qiskit quantum circuit code using Claude models as the code generator.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Sonnet 4 · Claude Opus 4 · Qiskit · Claude Code</p>

### DeepTruthSeek
*February 2025*

DeepSeek-r1-Llama-70B fine tune to improve detection and description of logical fallacies in written text. Used the CoCoLoFa dataset and PyTorch Fully Sharded Data Parallel (FSDP) training.

<p class="ai-tools"><strong>AI Tools:</strong> DeepSeek-r1-Llama-70B · PyTorch FSDP · CoCoLoFa Dataset · Claude Code</p>

## AI Agents & Visualization

### [Agent Blockchain Visualization](https://github.com/jknoll/agent-blockchain-visualization)
*2025*

Intelligent agent that analyzes blockchain security incidents and generates interactive 3D visualizations of transaction flows, attack patterns, and fund movements.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Agent SDK · TRM Labs BlockInt API · Three.js · Claude Code</p>

### [ClaudeCAD](https://github.com/jknoll/claude-cad)
*May 2025*

Connects Claude Desktop to a locally hosted Blender MCP server for 3D model generation from historical USPTO technical drawings. Name a historical mechanism (Wright Brothers Flyer, planetary gearbox, etc.) and Claude generates a 3D model from 2D drawings, with interactive parameter modification.

Built at the Y Combinator/Anthropic World's Largest MCP Hackathon. [DevPost](https://devpost.com/software/claudecad)

<p class="ai-tools"><strong>AI Tools:</strong> Claude Desktop · Blender MCP Server · Custom Technical Drawing MCP Server · Claude Code</p>

## Hackathon Projects

### Multimodal/Video Hackathon (Best Technical Execution)
*April 2025*

Realtime AI-enabled video avatar for conversational assistance in scheduling and administrative tasks. OIX and Susa Ventures.

[Deck](https://docs.google.com/presentation/d/1jZF_6TXdiOqh2s5y09uweuin3X02PdXXMVHmA6i6Cko/edit)

<p class="ai-tools"><strong>AI Tools:</strong> ByteDance LatentSync 1.5 · Sesame CSM (Conversational Speech Model) · Google Calendar API · WebAudio API · Mavi Transcription API</p>

### Anthropic Claude Plays Pokémon Hackathon (Grand Prize Winner)
*March 2025*

Pokémon playing agent competing against 120+ hackers. Optimized via agent prompt engineering, vision coordinate overlays, tool splitting/sub-specialization, and alternative context compression algorithms.

<p class="ai-tools"><strong>AI Tools:</strong> Claude 3.7 Sonnet · Vision Coordinate Overlays · Claude Code</p>

### ARC-AGI Hackathon ($10K Grant Recipient)
*September 2024*

Approach to the $1M ARC-AGI Challenge. Explored CNNs, autoencoders, language models, program generation, and ARC-DSL domain specific language. Proposed use of the Peano formal theorem proving environment.

<p class="ai-tools"><strong>AI Tools:</strong> CNNs · Autoencoders · Language Models · Peano Theorem Proving · Claude Code</p>

### Nous Research Atropos RL Environments Hackathon
*May 2025*

Distributed reinforcement learning environment within the Nous Research Atropos framework. Generated 1K conversational samples with (preferred, dispreferred) response pairs for DPO training of conversational models.

[Deck](https://docs.google.com/presentation/d/1s1xLnoPEATmgy1S0MrFJ9xdsFAA1XhNOsAkkgVaMlIE/edit)

<p class="ai-tools"><strong>AI Tools:</strong> DPO Training · Nous Research Atropos Framework · Claude Code</p>

## Claude Code Developer Tools

### [Claude Alarm Clock](https://github.com/jknoll/Claude-Alarm-Clock)
*2025*

Automated health monitoring and usage statistics collection for Claude Code CLI. Collects metrics and pipes them into BigQuery for analytics dashboards.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Code · ccusage · Google BigQuery · Looker Studio</p>

### [Multihost Utils](https://github.com/jknoll/multihost-utils)
*2025*

Session handoff, pickup, and permission sharing utilities for multi-host Claude Code workflows. Enables seamless work transfer between machines and web sessions.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Code</p>

### [GrooveLab](https://github.com/jknoll/stubblefield)
*2025*

Browser-based drum practice game using Web MIDI API. Connects to electronic drum kits and provides real-time feedback, scoring, and progress tracking. Built entirely with Claude Code.

<p class="ai-tools"><strong>AI Tools:</strong> Claude Code · Web MIDI API · Firebase</p>

## AI Tools Summary

### Large Language Models

| Model | Provider | Projects |
|:--|:--|:--|
| Claude Opus 4.6 | Anthropic | Clinical Trial Compass, Accessible Now |
| Claude Sonnet 4.5 | Anthropic | Clinical Trial Compass, Accessible Now |
| Claude Haiku 4.5 | Anthropic | Clinical Trial Compass |
| Claude Agent SDK | Anthropic | AdFlow, Agent Blockchain Visualization |
| Claude 3.7 Sonnet | Anthropic | Claude Plays Pokémon |
| Claude Sonnet 4 / Opus 4 | Anthropic | QuantumBench |
| Claude API | Anthropic | Claude Strudel |
| DeepSeek-r1-Llama-70B | DeepSeek | DeepTruthSeek |

### Video Generation

| Model | Provider | Projects |
|:--|:--|:--|
| Veo 3 Fast | Google (via Kie.ai) | AdFlow |
| Veo 3 Quality | Google (via Kie.ai) | AdFlow |
| WAN 2.6 (720p / 1080p) | FreePik | AdFlow |
| ByteDance LatentSync 1.5 | ByteDance | Multimodal/Video Hackathon |

### Image Generation

| Model | Provider | Projects |
|:--|:--|:--|
| Nano Banana Pro (Gemini 3 Pro Image) | Google (via Kie.ai) | Fakecation |

### Computer Vision & Transformers

| Model | Provider | Projects |
|:--|:--|:--|
| BEiT Vision Transformer (87.9M params) | Microsoft | FungiTastic |
| PyTorch CNN / ResNet / Transformer | Meta (PyTorch) | Chess AI, Chess Theme Classifier |

### Speech & Audio

| Model | Provider | Projects |
|:--|:--|:--|
| Sesame CSM | Sesame | Multimodal/Video Hackathon |
| Mavi Transcription API | Mavi | Multimodal/Video Hackathon |

### 3D Modeling & Visualization

| Tool | Provider | Projects |
|:--|:--|:--|
| Blender MCP Server | Blender Foundation | ClaudeCAD |
| Three.js | Open Source | Agent Blockchain Visualization |

### ML Infrastructure & Monitoring

| Tool | Provider | Projects |
|:--|:--|:--|
| Strong Compute ISC (72xA100) | Strong Compute | Chess AI, FungiTastic |
| Weights & Biases | Weights & Biases | FungiTastic, Chess Theme Classifier |
| TensorBoard | Google | Chess Theme Classifier |
| PyTorch FSDP | Meta | DeepTruthSeek |
| Google BigQuery / Looker Studio | Google | Claude Alarm Clock |
| Qiskit | IBM | QuantumBench |

### Web Extraction & Data APIs

| Tool | Provider | Projects |
|:--|:--|:--|
| TinyFish / Mino AI | Mino AI | AdFlow |
| TRM Labs BlockInt API | TRM Labs | Agent Blockchain Visualization |
| ClinicalTrials.gov API | NIH | Clinical Trial Compass |
| openFDA API | FDA | Clinical Trial Compass |
| Cloudinary | Cloudinary | Fakecation |

### Development

| Tool | Projects |
|:--|:--|
| Claude Code | All projects on this page |
