# Awesome Agentic Skills Research Papers

> A curated academic reading list on agentic skills: reusable procedural artifacts, skill libraries, routing, acquisition, evaluation, and governance for LLM-based agents.

Last checked: 2026-06-01.

## Scope

This repository is research-first. It is intentionally different from implementation catalogs such as `awesome-agent-skills` repositories that list ready-to-install `SKILL.md` packages.

Included:

- Papers where agent skills, skill libraries, skill routing, skill distillation, skill evolution, or skill evaluation are a primary object of study.
- Closely related precursor papers on tool learning, experiential learning, and executable skill libraries.
- Surveys, benchmarks, datasets, and security/governance papers that help define the field.

Not included by default:

- General LLM agent papers unless they introduce or evaluate reusable skills.
- Marketplaces or skill-package collections unless they are used as research artifacts.
- Prompt libraries with no evaluation or research contribution.

## Contents

- [Surveys and Position Papers](#surveys-and-position-papers)
- [Foundations and Precursors](#foundations-and-precursors)
- [Skill Acquisition and Self-Improvement](#skill-acquisition-and-self-improvement)
- [Skill Retrieval, Routing, and Context Construction](#skill-retrieval-routing-and-context-construction)
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Application-Specific Skill Systems](#application-specific-skill-systems)
- [Security and Governance](#security-and-governance)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)

## Surveys and Position Papers

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2026 | SoK: Agentic Skills -- Beyond Tool Use in LLM Agents | [arXiv](https://arxiv.org/abs/2602.20867) | Frames skills as reusable procedural capabilities beyond atomic tool calls, with lifecycle, representation, scope, and security taxonomies. |
| 2026 | Agent Skills for Large Language Models: Architecture, Acquisition, Security, and the Path Forward | [arXiv](https://arxiv.org/abs/2602.12430) | Focuses on the SKILL.md/progressive-disclosure abstraction, MCP relationship, acquisition, deployment, and trust tiers. |
| 2026 | A Comprehensive Survey on Agent Skills: Taxonomy, Techniques, and Applications | [arXiv](https://arxiv.org/abs/2605.07358) | Organizes the literature around representation, acquisition, retrieval, and evolution. |
| 2025 | LLM-Based Agents for Tool Learning: A Survey | [Springer](https://link.springer.com/article/10.1007/s41019-025-00296-9) | Useful bridge from tool learning to skill-equipped agents. |
| 2024 | A Review of Prominent Paradigms for LLM-Based Agents: Tool Use, Planning, and Feedback Learning | [arXiv](https://arxiv.org/abs/2406.05804) | Provides the broader agent paradigm background for skill-based systems. |
| 2023 | A Survey on Large Language Model based Autonomous Agents | [arXiv](https://arxiv.org/abs/2308.11432) | General LLM-agent survey; useful for positioning skills against memory, planning, and action modules. |
| 2023 | The Rise and Potential of Large Language Model Based Agents: A Survey | [arXiv](https://arxiv.org/abs/2309.07864) | Broad overview of single-agent, multi-agent, and human-agent scenarios. |

## Foundations and Precursors

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2023 | Toolformer: Language Models Can Teach Themselves to Use Tools | [arXiv](https://arxiv.org/abs/2302.04761) | Early self-supervised tool-use training; a precursor to learning callable procedural capability. |
| 2023 | API-Bank: A Comprehensive Benchmark for Tool-Augmented LLMs | [arXiv](https://arxiv.org/abs/2304.08244) | Benchmark and dataset for tool-augmented LLM behavior. |
| 2023 | On the Tool Manipulation Capability of Open-source Large Language Models | [arXiv](https://arxiv.org/abs/2305.16504) | Studies practical tool manipulation and creates a ToolBench benchmark. |
| 2023 | ToolLLM: Facilitating Large Language Models to Master 16000+ Real-world APIs | [arXiv](https://arxiv.org/abs/2307.16789) | Large-scale API/tool learning framework and dataset. |
| 2023 | Voyager: An Open-Ended Embodied Agent with Large Language Models | [arXiv](https://arxiv.org/abs/2305.16291) | Introduces an ever-growing executable code skill library for Minecraft agents. |
| 2023 | ExpeL: LLM Agents Are Experiential Learners | [arXiv](https://arxiv.org/abs/2308.10144) | Learns from task experience without model-weight updates; important precursor to skill distillation. |
| 2024 | SkillAct: Using Skill Abstractions Improves LLM Agents | [OpenReview](https://openreview.net/forum?id=6LG3cIRrF4) | Shows that prompting with reusable skill abstractions improves interactive task performance. |
| 2024 | LLMs in the Imaginarium: Tool Learning through Simulated Trial and Error | [arXiv](https://arxiv.org/abs/2403.04746) | Uses simulated trial-and-error and memory to learn tool use behavior. |

## Skill Acquisition and Self-Improvement

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2024 | Agentic Skill Discovery | [arXiv](https://arxiv.org/abs/2405.15019) | LLM-driven discovery of robotic skills from zero initial skill library. |
| 2025 | Reinforcement Learning for Self-Improving Agent with Skill Library | [arXiv](https://arxiv.org/abs/2512.17102) | Introduces SAGE, using Skill Augmented GRPO and sequential rollouts to accumulate reusable skills. |
| 2025 | CASCADE: Cumulative Agentic Skill Creation through Autonomous Development and Evolution | [arXiv](https://arxiv.org/abs/2512.23880) | Studies cumulative skill creation and evolution for AI-assisted scientific workflows. |
| 2026 | SkillRL: Evolving Agents via Recursive Skill-Augmented Reinforcement Learning | [arXiv](https://arxiv.org/abs/2602.08234) | Builds a hierarchical SkillBank from experience and co-evolves skill library and policy. |
| 2026 | Agentic Proposing: Enhancing Large Language Model Reasoning via Compositional Skill Synthesis | [arXiv](https://arxiv.org/abs/2602.03279) | Uses modular reasoning skills to synthesize verifiable training problems. |
| 2026 | Skill-SD: Skill-Conditioned Self-Distillation for Multi-turn LLM Agents | [arXiv](https://arxiv.org/abs/2604.10674) | Converts agent trajectories into dynamic training-only skill supervision. |
| 2026 | SkillX: Automatically Constructing Skill Knowledge Bases for Agents | [arXiv](https://arxiv.org/abs/2604.04804) | Builds plug-and-play hierarchical skill knowledge bases from trajectories. |
| 2026 | Skill1: Unified Evolution of Skill-Augmented Agents via Reinforcement Learning | [arXiv](https://arxiv.org/abs/2605.06130) | Jointly optimizes skill selection, utilization, and distillation from a shared task-outcome signal. |
| 2026 | SkillGraph: Skill-Augmented Reinforcement Learning for Agents via Evolving Skill Graphs | [arXiv](https://arxiv.org/abs/2605.12039) | Represents skills as graph nodes with prerequisite, enhancement, and co-occurrence edges. |
| 2026 | SkillMaster: Toward Autonomous Skill Mastery in LLM Agents | [arXiv](https://arxiv.org/abs/2605.08693) | Trains agents to create, refine, and select their own accumulated skills. |
| 2026 | COLLEAGUE.SKILL: Automated AI Skill Generation via Expert Knowledge Distillation | [arXiv](https://arxiv.org/abs/2605.31264) | Distills person- or role-grounded traces into inspectable, correctable skill packages. |

## Skill Retrieval, Routing, and Context Construction

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2026 | SkillRouter: Retrieve-and-Rerank Skill Selection for LLM Agents at Scale | [arXiv](https://arxiv.org/abs/2603.22455) | Studies large-scale skill routing and shows full skill bodies are crucial routing signal. |
| 2026 | Graph-of-Skills: Dependency-Aware Structural Retrieval for Massive Agent Skills | [arXiv](https://arxiv.org/abs/2604.05333) | Retrieves dependency-aware skill bundles instead of isolated semantically similar skills. |
| 2026 | SkillsInjector: Dynamic Skill Context Construction for LLM Agents | [arXiv](https://arxiv.org/abs/2605.29794) | Learns adaptive skill budgets and set-aware rendering for injected context. |
| 2026 | The Scaling Laws of Skills in LLM Agent Systems | [arXiv](https://arxiv.org/abs/2605.16508) | Empirically studies how routing and execution degrade or recover as skill libraries scale. |

## Benchmarks and Evaluation

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2026 | How Well Do Agentic Skills Work in the Wild: Benchmarking LLM Skill Usage in Realistic Settings | [arXiv](https://arxiv.org/abs/2604.04323) | Benchmarks skill utility under realistic retrieval and refinement conditions. |
| 2026 | SkillRet: A Large-Scale Benchmark for Skill Retrieval in LLM Agents | [arXiv](https://arxiv.org/abs/2605.05726) | Provides a retrieval benchmark with public agent skills, taxonomy, training samples, and evaluation queries. |
| 2026 | SkillMOO: Multi-Objective Optimization of Agent Skills for Software Engineering | [arXiv](https://arxiv.org/abs/2604.09297) | Optimizes SE skill bundles for both pass rate and inference cost. |
| 2026 | ClawTrace: Cost-Aware Tracing for LLM Agent Skill Distillation | [arXiv](https://arxiv.org/abs/2604.23853) | Adds cost-aware trace cards and skill patches for distillation pipelines. |

## Application-Specific Skill Systems

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2026 | CUA-Skill: Develop Skills for Computer Using Agent | [arXiv](https://arxiv.org/abs/2601.21123) | Builds a structured skill base for computer-using agents on Windows applications. |
| 2026 | PANDO: Efficient Multimodal AI Agents via Online Skill Distillation | [arXiv](https://arxiv.org/abs/2605.24785) | Online skill distillation for multimodal web agents with efficiency metrics. |
| 2026 | SkillMOO: Multi-Objective Optimization of Agent Skills for Software Engineering | [arXiv](https://arxiv.org/abs/2604.09297) | Software-engineering-specific skill-bundle search and cost optimization. |
| 2024 | Agentic Skill Discovery | [arXiv](https://arxiv.org/abs/2405.15019) | Robotics-oriented skill discovery driven by LLM task proposals and RL. |
| 2023 | Voyager: An Open-Ended Embodied Agent with Large Language Models | [arXiv](https://arxiv.org/abs/2305.16291) | Embodied open-world skill library with executable code skills. |

## Security and Governance

| Year | Paper | Links | Why it matters |
| --- | --- | --- | --- |
| 2026 | SoK: Agentic Skills -- Beyond Tool Use in LLM Agents | [arXiv](https://arxiv.org/abs/2602.20867) | Discusses supply-chain risk, prompt injection through skills, malicious skill payloads, and trust-tiered execution. |
| 2026 | Agent Skills for Large Language Models: Architecture, Acquisition, Security, and the Path Forward | [arXiv](https://arxiv.org/abs/2602.12430) | Proposes a Skill Trust and Lifecycle Governance Framework. |
| 2026 | How Well Do Agentic Skills Work in the Wild | [arXiv](https://arxiv.org/abs/2604.04323) | Shows the fragility of skill gains under realistic retrieval and refinement conditions. |

## Related Awesome Lists

These are useful, but have a different center of gravity from this repository.

- [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) - implementation-oriented skill catalog.
- [kodustech/awesome-agent-skills](https://github.com/kodustech/awesome-agent-skills) - engineering skill catalog.
- [JayLZhou/Awesome-Agent-Skills](https://github.com/JayLZhou/Awesome-Agent-Skills) - companion resources for a survey on agent skills.
- [baibizhe/Awesome-Skills-Paper](https://github.com/baibizhe/Awesome-Skills-Paper) - existing paper list; this repo aims for a research-map style taxonomy and stricter scope notes.
- [Paitesanshi/LLM-Agent-Survey](https://github.com/Paitesanshi/LLM-Agent-Survey) - broader LLM-agent survey resources.
- [WooooDyy/LLM-Agent-Paper-List](https://github.com/WooooDyy/LLM-Agent-Paper-List) - broad LLM-agent paper list.

## Contributing

Please open an issue or pull request if a relevant paper is missing.

Suggested entry format:

```markdown
| 2026 | Paper Title | [arXiv](https://arxiv.org/abs/xxxx.xxxxx) / [Code](https://github.com/...) | One-sentence reason this belongs in agentic skill research. |
```

Inclusion checklist:

- The paper treats skills, reusable procedures, tool-using routines, executable behaviors, skill libraries, or skill routing as a main contribution.
- The link points to a primary source when possible: arXiv, ACL Anthology, OpenReview, publisher page, project page, or official repository.
- The note explains the agentic-skill relevance, not just the general LLM-agent relevance.
