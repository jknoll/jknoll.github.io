---
title: Justin F. Knoll
layout: default
author: Justin F. Knoll
profile_image: profile-400.jpg
---

<div class="profile-section">
  <img src="{{ page.profile_image }}" alt="Profile Photo" class="profile-photo" style="width: 200px; height: 200px; border-radius: 50%; object-fit: cover;">
</div>

## Introduction

I've recently conducted an artificial intelligence and machine learning deep dive, hands-on coding and hackathon competition as a way to create tangible implementations and connect with others in the industry. Over the course of this deep dive, I've been able to compete in a broad spectrum of competitions, tally a number of wins, and accumulate more than $42,000 in GPU and API prize credits in a short time.

## AI and ML Hackathons and Projects

### Chess AI Hackathon Series (Six-Time Winner | Python, PyTorch, NumPy, Cluster Training)
August, 2024-March, 2025

Formed and led a team of three in competition against ten San Francisco and Sydney teams to build the strongest possible chess-playing deep learning model in only two days. Sponsored by Strong Compute (YC W22)

Explored two high-level approaches: a vision-like CNN model and a language-like GPT model. A key inspiration for the GPT-based models was Adam Karvonen's paper [Emergent World Models and Latent Variable Estimation in Chess-Playing Language Models](https://arxiv.org/abs/2403.15498). Within the vision approach, we experimented with CNNs, dilated convolution, ResNets, transformers, and multi-head self-attention. Trained on a 72xA100 cluster. Won the first tournament with a record of 8 wins, 1 loss, 1 draw, earning a $10K GPU compute credit. Released model source code and a case study.

Returned as a solo entrant to win five out of six subsequent instances of the tournament.

### Chess Theme and Opening Multilabel Classifier (Grant Recipient)
April 2025-July 2025

Research project to implement a deep convolutional neural network to perform multi-label classification of board positions sourced from the lichess puzzles dataset. Each board position is labeled with applicable themes (for example, back rank mate, zugzwang, advanced pawn, etc.) as well as openings, if relevant (for example, Sicilian Defense, The English Opening, etc.)

A model is trained to recognize the positions and themes and then to apply the same classification mechanism to positions during live games or during review of unseen games.

### ARC-AGI Hackathon (Grant Recipient | ARC-DSL, Peano)
September, 2024

Formed a team of three to develop and pitch an approach to the $1M ARC-AGI Challenge (Abstraction and Reasoning Corpus for Artificial General Intelligence). Explored CNNs, Autoencoders, language models, and program generation. Investigated ARC-DSL domain specific language. Ultimately proposed use of the Peano formal theorem proving environment. Awarded a $10K research grant.

### DeepTruthSeek (PyTorch, SFT, LoRA, FSDP training)
February, 2025

Project to create a DeepSeek-r1-Llama-70B fine tune to improve detection and description of logical fallacies in written text. Used the CoCoLoFa dataset from "CoCoLoFa: A Dataset of News Comments with Common Logical Fallacies Written by LLM-Assisted Crowds" and PyTorch Fully Sharded Data Parallel (FSDP) training.

### Anthropic Claude Plays Pokémon Hackathon (Grand Prize Winner | Agents, Claude 3.7 Sonnet)
March, 2025

Formed a team and competed against 120+ hackers to create the best Pokémon playing agent based on Claude 3.7 Sonnet, determined by distance-from-origin progress through a notoriously challenging level as the objective function. Experimented with agent prompt engineering, vision coordinate overlays, splitting/sub-specialization of tools, and alternative context compression algorithms.

### Multimodal/Video Hackathon, OIX and Susa Ventures (Winner: Best Technical Execution)
April, 2025

Created a realtime AI-enabled video avatar for conversational assistance in scheduling and other administrative tasks. Implemented a solution using ByteDance LatentSync 1.5 for video/audio lip synchronization, Sesame CSM (Conversational Speech Model) for realistic text-to-speech, Google Calendar API for scheduling and the WebAudio API and Mavi Transcription APIs for capturing user questions for the agent via browser microphone input.

[Deck](https://docs.google.com/presentation/d/1jZF_6TXdiOqh2s5y09uweuin3X02PdXXMVHmA6i6Cko/edit?slide=id.g3391f583a3c_0_0#slide=id.g3391f583a3c_0_0)

### Y Combinator/Anthropic World's Largest MCP Hackathon
May, 2025

Built a project which connects Claude Desktop to a locally hosted Blender MCP server, a local Blender instance, and a newly-developed local MCP server which serves as a technical drawing database and server for USPTO technical drawing.

The user can name a historical engineering mechanism or artifact. For example, the Wright Brothers Flyer, a planetary gearbox, etc. Claude then generates a 3D model directly from the 2D technical drawings. The user can modify the model by changing parameters, materials, etc., and can ask for information about the model's mechanism, function, and effects of any modifications.

[Link](https://devpost.com/software/claudecad)

### Nous Research Atropos RL Environments Hackathon (Distributed RL)
May, 2025

Created an environment for distributed reinforcement learning within the Nous Research [Atropos](https://github.com/NousResearch/atropos) framework. Generated a set of 1K conversational samples with (preferred, dispreferred) response pairs via a meta-prompt. Used these response pairs for DPO training of conversational models to align with individual user preferences in tone, politeness, etc.

[Deck](https://docs.google.com/presentation/d/1s1xLnoPEATmgy1S0MrFJ9xdsFAA1XhNOsAkkgVaMlIE/edit?slide=id.g35a3b68de50_0_1097#slide=id.g35a3b68de50_0_1097)

## Professional Certifications

<style>
.cert-table { width: 100%; border-collapse: collapse; margin: 1em 0; }
.cert-table th, .cert-table td { padding: 8px 12px; text-align: left; border-bottom: 1px solid #e1e1e1; }
.cert-table th { font-weight: 600; }
.cert-icon { width: 20px; height: 20px; vertical-align: middle; margin-right: 6px; }
.cert-issuer { display: flex; align-items: center; }
</style>

### AI & LLM Development

| Certification | Issuer | Date | |
|:--|:--|:--|:--|
| Google Cloud Attention Mechanism | <img src="https://www.google.com/favicon.ico" class="cert-icon" alt="Google">Google | Dec 2025 | [Credential](https://www.skills.google/public_profiles/6e55b6c6-6fb3-4817-8af0-3b3c606f00c2/badges/21077514) |
| Google Cloud Introduction to Image Generation | <img src="https://www.google.com/favicon.ico" class="cert-icon" alt="Google">Google | Dec 2025 | [Credential](https://www.skills.google/public_profiles/6e55b6c6-6fb3-4817-8af0-3b3c606f00c2/badges/21077468) |
| Introduction to Model Context Protocol | <img src="https://www.anthropic.com/favicon.ico" class="cert-icon" alt="Anthropic">Anthropic | Dec 2025 | [Credential](https://verify.skilljar.com/c/gof5dqdep7jb) |
| Building with the Claude API | <img src="https://www.anthropic.com/favicon.ico" class="cert-icon" alt="Anthropic">Anthropic | Nov 2025 | [Credential](https://verify.skilljar.com/c/vdtotcggcu9c) |
| Claude Code in Action | <img src="https://www.anthropic.com/favicon.ico" class="cert-icon" alt="Anthropic">Anthropic | Nov 2025 | [Credential](https://verify.skilljar.com/c/ud93e5ugyay7) |
| LangChain Essentials – Python | <img src="https://python.langchain.com/img/favicon.ico" class="cert-icon" alt="LangChain">LangChain | Nov 2025 | [Credential](https://academy.langchain.com/certificates/mdoxpdfcxu) |
| LangGraph Essentials – Python | <img src="https://python.langchain.com/img/favicon.ico" class="cert-icon" alt="LangChain">LangChain | Nov 2025 | [Credential](https://academy.langchain.com/certificates/n1gd9f4jqk) |
| Neural Networks and Deep Learning | <img src="https://www.deeplearning.ai/favicon.ico" class="cert-icon" alt="DeepLearning.AI">DeepLearning.AI | Oct 2020 | [Credential](http://coursera.org/verify/QK88DVWS3N2Q) |

### Product & Process

| Certification | Issuer | Date | |
|:--|:--|:--|:--|
| Inspired: How to Create Tech Products Customers Love | <img src="https://www.svpg.com/favicon.ico" class="cert-icon" alt="SVPG">SVPG | Apr 2015 | |
| Certified ScrumMaster | <img src="https://www.scrumalliance.org/favicon.ico" class="cert-icon" alt="Scrum Alliance">Scrum Alliance | Oct 2008 | |

## Professional Skills

### AI & Machine Learning

**Attention Mechanism**
- Expertise in transformer attention layers, including self-attention, cross-attention, and their role in sequence modeling, scaling laws, and modern LLM architectures.
- *Associated With:* Google Cloud Attention Mechanism

**Diffusion Models**
- Experience with diffusion-based generative modeling, including denoising diffusion probabilistic models (DDPMs), latent diffusion, and text-to-image systems.
- *Associated With:* Google Cloud Introduction to Image Generation

**Large Language Models (LLMs)**
- Architecture, training paradigms, inference optimization, evaluation, and deployment of transformer-based language models.
- *Associated With:* Anthropic Claude, LangChain, Google Cloud, DeepLearning.AI

**Transformers**
- Encoder-decoder models, self-attention scaling, positional encoding, and pretraining/fine-tuning dynamics.
- *Associated With:* Google Cloud Attention Mechanism, DeepLearning.AI

**Deep Learning**
- CNNs, RNNs, optimization, regularization, representation learning, and large-scale training.
- *Associated With:* Stanford University, DeepLearning.AI

**Machine Learning**
- Supervised, unsupervised, and reinforcement learning; model evaluation; feature engineering; production ML systems.

### AI Agents & Orchestration

**AI Agents**
- Building autonomous and semi-autonomous LLM agents, including tool use, planning, memory, state machines, and human-in-the-loop workflows.
- *Associated With:* LangGraph, LangChain, Claude API, Claude Code

**Coding Agents**
- Use of LLM-driven coding agents for repo navigation, refactoring, cross-file reasoning, test generation, and large-scale code transformation.
- *Associated With:* Claude Code in Action

**Model Context Protocol (MCP)**
- Design and use of MCP servers and clients to provide secure, structured tool and data access for LLM agents.
- *Associated With:* Anthropic – Introduction to MCP, Claude Code in Action

**LangChain**
- Chains, agents, tools, retrievers, memory, LangSmith observability, and modular LLM application design.
- *Associated With:* LangChain Essentials – Python

**LangGraph**
- Graph-based control flow for multi-actor, cyclic, and long-running LLM workflows with durable state and human oversight.
- *Associated With:* LangGraph Essentials – Python

**Prompt Engineering**
- Designing structured prompts, tool schemas, and conversation protocols for reliability, controllability, and reasoning depth.
- *Associated With:* Building with the Claude API

**Retrieval-Augmented Generation (RAG)**
- End-to-end RAG pipelines: embedding, chunking, vector search, hybrid retrieval, and grounding generation in proprietary knowledge bases.
- *Associated With:* Building with the Claude API

### Engineering & Systems

**Software Engineering**
- End-to-end software lifecycle: architecture, implementation, testing, deployment, and operations.
- *Includes:* GitHub, CI/CD, Distributed Systems, Algorithm Design, Unix

**Distributed Systems**
- Scalable, fault-tolerant architectures, data pipelines, and large-scale backend systems.

**Cloud Applications**
- Designing and operating cloud-native, high-throughput, globally distributed services.
- *Associated With:* Google Cloud, BitTorrent

**Data & Analytics**
- Designing metrics systems, analytical pipelines, and executive dashboards for product and research insights.
- *Includes:* SQL, Big Data Analytics, Dashboard Metrics, Statistical Data Analysis, Data Visualization

### Web3 & Product

**Web3 / Blockchain**
- Ethereum ecosystem, wallets, smart contracts, DAOs, zero-knowledge systems, and cryptographic infrastructure.
- *Associated With:* Consensys, MetaMask

**Product Management**
- Product strategy, OKRs, roadmapping, execution, growth, and cross-functional alignment for zero-to-one and scale products.

**Developer Relations**
- API platforms, SDKs, community growth, technical evangelism, and developer experience.
- *Associated With:* MetaMask

<!--
## Publications
(No publications data provided)

## Teaching
(No teaching data provided)

## Talks & Presentations
(Presentations linked in project descriptions above)

## Portfolio
(See AI and ML Hackathons and Projects section above)

## Blog Posts
(No blog posts data provided)

## CV
(Skills and certifications included in sections above)
-->
