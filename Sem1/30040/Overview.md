# Thrid Year Project - Agentic LLM-based model for investment analysis reasoning

## Motivation
Individual analysts and portfolio managers routinely sift through thousands of pages of earnings reports, macro-economic data, and market commentary to form a coherent investment thesis. Large-language models (LLMs) now rival domain experts in linguistic comprehension, yet their outputs remain opaque and hard to audit. By wrapping an LLM in an agentic architecture, one that includes explicit reasoning traces and direct access to primary data sources (structured and unstructured), we can deliver a model which can operate as an investment analysis co-pilot.

## Project Description
The project will build a multi-agent LLM system dedicated to informal (human-readable) investment reasoning rather than automated trading execution. A central Analyst Agent receives a high-level query, e.g. “Is Acme Corp. attractive at today’s valuation given a potential Fed rate cut this year?”, and proceeds through a transparent epistemically-informed Chain-of-Thought (CoT)-based analytical plan. Other agents enrich and critique this draft reasoning:

1. Data-Retrieval Agent: Queries structured fundamentals (income statements, cash-flow, key ratios), macro indicators (CPI, yield curves), and unstructured sources (10-K filings, earnings-call transcripts, news headlines) from a vector-indexed knowledge base. All excerpts are returned with source links and timestamps.
 

2. Risk-Assessment Agent: Applies lightweight formal-epistemology priors to every CoT step, assigning credence scores that reflect evidence strength, model uncertainty, and data timeliness.
 

3. Compliance Agent: Scans for regulatory red flags, ensuring adherence to SEC safe-harbour language and the firm’s internal disclosure policies.
 

The ensemble outputs a research memo: a Markdown / LaTeX document that interleaves narrative reasoning, tabular evidence, and dynamic “what-if” scenarios (e.g. EBIT sensitivity to WACC changes). A full-stack web application, React/TypeScript front end, FastAPI back end, lets users (i) launch new analyses, (ii) drill into any CoT node to inspect the underlying data slice, or (iii) revise premises and regenerate downstream reasoning. 

## Project Description
Recommended skills are: solid Python, familiarity with financial statements, basic probability/statistics, and modern web-development tooling. Previous courses on NLP and Symbolic AI are desirable.