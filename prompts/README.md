# Agent Prompts

This folder documents the system instructions configured for the three agents in the SketricGen workflow. The prompts define each agent's role, evidence boundaries, handoff rules, output requirements, and failure handling.

- [Lead Orchestration Agent](lead-orchestrator.md) — controls order of execution, validates research handoff, synthesizes the final brief, and checks citations.
- [SEO Research Analyst](seo-research-analyst.md) — gathers current evidence through web search and separates sourced findings from interpretation.
- [SEO Content Strategist](seo-content-strategist.md) — uses the research handoff to develop the SEO strategy without inventing evidence.

These files document prompts used in the SketricGen project. The repository does not include a standalone executable agent implementation. Before publishing the full prompt text publicly, confirm that your assessment terms or any confidentiality agreement do not restrict sharing your submitted prompt configuration.
