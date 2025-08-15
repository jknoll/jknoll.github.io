---
title: Justin F. Knoll Project Page
---
# Justin F. Knoll

I've recently conducted an artificial intelligence and machine learning deep dive, with hands-on coding and hackathon competition as a way to create tangible implementations and connect with others in the industry. Over the course of this deep dive, I've been able to compete in a broad spectrum of competitions, tally a number of wins, and accumulate more than $42,000 in GPU and API prize credits in a short time.

## Artificial Intelligence/Machine Learning Hackathons and Projects

### Chess AI Hackathon (Winner 6x | Python, PyTorch, NumPy, Cluster Training)
August, 2024-March, 2025

Formed and led a team of three in competition against ten San Francisco and Sydney teams to build the strongest possible chess-playing deep learning model in only two days. Sponsored by Strong Compute (YC W22) 

Explored two high-level approaches: a vision-like CNN model and a language-like GPT model. A key inspiration for the GPT-based models was Adam Karvonen’s paper [Emergent World Models and Latent Variable Estimation in Chess-Playing Language Models](https://arxiv.org/abs/2403.15498). Within the vision approach, we experimented with CNNs, dilated convolution, ResNets, transformers, and multi-head self-attention. Trained on a 72xA100 cluster. Won the first tournament with a record of 8 wins, 1 loss, 1 draw, earning a $10K GPU compute credit. Released model source code and a case study.

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

Project to create a DeepSeek-r1-Llama-70B fine tune to improve detection and description of logical fallacies in written text. Used the CoCoLoFa dataset from ”CoCoLoFa: A Dataset of News Comments with Common Logical Fallacies Written by LLM-Assisted Crowds” and PyTorch Fully Sharded Data Parallel (FSDP) training.

### Anthropic Claude Plays Pokémon Hackathon (Grand Prize Winner | Agents, Claude 3.7 Sonnet)
March, 2025

Formed a team and competed against 120+ hackers to create the best Pokémon playing agent based on Claude 3.7 Sonnet, determined by distance-from-origin progress through a notoriously challenging level as the objective function. Experimented with agent prompt engineering, vision coordinate overlays, splitting/sub-specialization of tools, and alternative context compression algorithms.

### Multimodal/Video Hackathon, OIX and Susa Ventures (Winner: Best Technical Execution| LatentSync, Sesame CSM)
April, 2025

Created a realtime AI-enabled video avatar for conversational assistance in scheduling and other administrative tasks. Implemented a solution using ByteDance LatentSync 1.5 for video/audio lip synchronization, Sesame CSM (Conversational Speech Model) for realistic text-to-speech, Google Calendar API for scheduling and the WebAudio API and Mavi Transcription APIs for capturing user questions for the agent via browser microphone input.

[Deck](https://docs.google.com/presentation/d/1jZF_6TXdiOqh2s5y09uweuin3X02PdXXMVHmA6i6Cko/edit?slide=id.g3391f583a3c_0_0#slide=id.g3391f583a3c_0_0)

### Y Combinator/Anthropic World's Largest MCP Hackathon
May, 2025

Built a project which connects Claude Desktop to a locally hosted Blender MCP server, a local Blender instance, and a newly-developed local MCP server which serves as a technical drawing database and server for USPTO technical drawing.

The user can name a historical engineering mechanism or artifact. For example, the Wright Brothers Flyer, a planetary gearbox, etc. Claude then generates a 3D model directly from the 2D technical drawings. The user can modify the model by changing parameters, materials, etc., and can ask for information about the model's mechanism, function, and effects of any modifications.

[Link](https://devpost.com/software/claudecad)

### Nous Research Atropos RL Environments Hackathon (Distributed Reinforcement Learning)
May, 2025

Created an environment for distributed reinforcement learning within the Nous Research [Atropos](https://github.com/NousResearch/atropos) framework. Generated a set of 1K conversational samples with (preferred, dispreferred) response pairs via a meta-prompt. Used these response pairs for DPO training of conversational models to align with individual user preferences in tone, politeness, etc. 

[Deck](https://docs.google.com/presentation/d/1s1xLnoPEATmgy1S0MrFJ9xdsFAA1XhNOsAkkgVaMlIE/edit?slide=id.g35a3b68de50_0_1097#slide=id.g35a3b68de50_0_1097)
