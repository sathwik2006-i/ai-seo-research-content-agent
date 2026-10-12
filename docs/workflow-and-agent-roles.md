# Workflow and Agent Responsibilities

## Purpose

The workflow turns a user's topic, target audience, market/location, and content objective into a concise SEO content brief backed by traceable web research. It separates evidence gathering from strategy so that strategic recommendations are grounded in the research collected for the current request.

## Execution sequence

1. **Parse the request.** The lead agent identifies the topic, target audience, market, objective, and requested format.
2. **Run research.** The SEO Research Analyst searches for relevant, current information, observed competitor/content coverage, audience questions, evidence-backed gaps, and source references.
3. **Validate the research handoff.** The lead agent checks that the returned material contains actual findings, not merely a completion message or empty response. If the research is not usable, the workflow should explain the limitation rather than fabricate a strategy.
4. **Generate strategy.** The SEO Content Strategist receives the original request and the research findings. It develops search intent, a primary keyword or topic phrase, supporting terms, title, content angle, structure, differentiation opportunities, and a call to action.
5. **Synthesize the brief.** The lead agent reconciles the research and strategy, removes unsupported claims, preserves source numbering, and marks inferences/recommendations.
6. **Check the final format.** The output is organized into 14 sections so a writer can review and use it.

## Agent responsibilities

### Lead Orchestration Agent

- Coordinates the order of operations.
- Validates the research output before strategy begins.
- Passes the full usable research output to the strategist.
- Synthesizes the strategy with the research findings.
- Audits claim-to-source alignment and labels inferences or recommendations.

### SEO Research Analyst

- Uses the connected web-search capability to gather current information.
- Identifies relevant facts, source references, audience questions, and observed content gaps.
- Distinguishes sourced findings from interpretation.
- Does not own the final content strategy or final brief.

### SEO Content Strategist

- Uses the research handoff as its factual basis.
- Recommends search intent, keywords/topic phrases, title, content angle, outline, and differentiation opportunities.
- Avoids presenting an inferred topic phrase as a proven high-demand keyword when keyword-volume/difficulty data is unavailable.
- Does not perform separate research in the documented design.

## Models and tool configuration

The assessment describes GPT-4.1 Mini for all three agents. The SEO Research Analyst has Web Search; the lead and strategist have no separate tools configured in the assessment.

## Expected final sections

The configured output format has 14 sections: topic, target audience, market/location, search intent, primary keyword, secondary keywords, recommended title, content angle, suggested article structure, key questions to answer, content gaps and differentiation opportunities, recommended call to action, assumptions made, and important sources.

## State and handoffs

The documented design relies on sequential handoffs: research must complete and be inspected before the strategist is invoked, and the research findings must be present in the strategist's input. The assessment does not establish durable task storage, checkpointing, or persistent memory for long-running jobs; those would be possible future enhancements rather than current capabilities claimed here.
