AIX Protocol
AI Experience — The Design Layer for Machine-Readable Research
> *The web was built for human eyes. This is what happens when you redesign it for AI.*
---
AIX (AI Experience) is to artificial intelligence what UX (User Experience) is to humans.
Every website, every Wikipedia page, every research paper online was designed for a human brain — navigation menus, footnotes, citation numbers, disambiguation links, sidebar ads. An AI fetching that same page gets all of it: the signal and the noise. It pays to process every token equally.
The result: AI agents waste 70–97% of their token budget just to find the 3–30% of content that actually answers the question.
AIX Protocol is a framework and a practical tool to fix that.
---
What's In This Repo
File	What It Is
`aix-skill.md`	The skill. Paste into your Claude Project to activate AIX.
`comparison-results.md`	The proof. Real before/after on Wikipedia's AGI page. 97% noise eliminated.
`aix-principles.md`	(Coming soon) The 7 core principles of AI Experience design.
---
The Problem (In Real Numbers)
When an AI fetches Wikipedia's AGI page without AIX:
~15,500 tokens loaded into context
~3,200 tokens actually useful (~21%)
~12,300 tokens are citation markers `[[1]]`, link syntax `[text](url)`, footnotes, "See also" lists, reference bibliographies, navigation headers
97% noise on one of the most popular research pages on earth
That's not a Wikipedia problem. Every major research site has the same issue — arXiv, PubMed, MDN, Stack Overflow.
See the full comparison: `comparison-results.md`
---
The Fix: AIX Skill for Claude
A Claude Project system prompt that instructs the model to:
Strip all noise — citation brackets, link syntax, nav elements, footnotes
Extract only signal — facts, definitions, timeline, current status, key people
Format for both humans and AI — structured sections + a JSON block for agents
Report efficiency — token count saved vs. raw fetch
Stay within a token budget — returns exactly what's needed, nothing more
What the output looks like
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━
TOPIC: Artificial General Intelligence (AGI)
QUERY: What is AGI? Research overview.
━━━━━━━━━━━━━━━━━━━━━━━━━━━

◆ DEFINITION
AGI is a type of AI that matches or surpasses human capabilities across
virtually all cognitive tasks.

◆ KEY FACTS
• Sam Altman declared in December 2025: "We built AGIs"
• Google DeepMind (2023) proposed 5 AGI levels: Emerging → Competent → Expert → Virtuoso → Superhuman
• 72 active AGI R&D projects across 37 countries (2020 survey)
[...]

◆ AIX EFFICIENCY
• Signal tokens delivered: ~480
• Estimated raw source size: ~15,500 tokens
• Noise eliminated: 97%
━━━━━━━━━━━━━━━━━━━━━━━━━━━
```
480 tokens instead of 15,500. Same research value. Zero noise.
---
How To Use It (No Coding Required)
For Claude.ai users:
Go to claude.ai
Create a new Project (sidebar → New Project)
Click Project Instructions
Open `aix-skill.md` in this repo
Copy everything under the `▼ PASTE FROM HERE` line
Paste into the Project Instructions field
Done. Every conversation in that project now runs under AIX Protocol.
For developers / AI agents:
Use the AIX format as a system prompt prefix for any research-oriented agent
The JSON block at the end of each response is structured for direct ingestion
Token budget rules are built in — no more context window blowouts from noisy fetches
---
Why This Matters Beyond Token Cost
This isn't just about saving money on API calls.
When AI agents do research today:
They get the same bloated, human-designed page every browser gets
They spend reasoning cycles just finding where the information is
Poorly structured content forces more inference steps, more errors, more hallucinations
Multi-source research multiplies the problem: 5 sources × 15,000 tokens = 75,000 tokens of mostly noise
Better signal in = better answers out.
The AIX Protocol is the first step toward a web that serves AI as a first-class reader — not an afterthought trying to scrape through content built for human eyes.
---
The Bigger Picture: AIX as a Field
UX (User Experience) started as an idea — the web should be designed for how humans actually use it. It became a field, a profession, a set of standards that now everyone follows.
AIX (AI Experience) is the same idea for machines.
As AI agents become research tools, autonomous workers, and infrastructure — the web needs to be redesigned with AI as a first-class reader. That means:
Content structure that AI can navigate semantically, not just visually
Data endpoints that serve AI agents differently from human browsers
Efficiency standards — an AIX score for how well a page serves AI consumption
Token budget awareness built into how content is published
This repo is the beginning of that standard. The skill is the first tool. The principles are next.
---
Comparison Results
Metric	Without AIX	With AIX
Tokens consumed (Wikipedia AGI)	~15,500	~480
Noise in response	~79%	~0%
Machine-readable output	❌	✅
Copy-paste ready for AI pipeline	❌	✅
Token cost saved per query	—	~97%
Full methodology and raw data: `comparison-results.md`
---
About
Concept & Design: Ashu Sehgal (@ashu-sehgal)
UX designer who noticed that the web was designed for human experience — and nobody had asked what AI experience should look like.
AIX is an attempt to coin that field, prove the gap is real, and build the first practical tool under it.
This project is intentionally open source. If the idea is right, it should belong to everyone.
---
Contribute
Test the skill on different research websites and report your token savings in Issues
Suggest improvements to the AIX Response Format
Help write the AIX Principles document (coming soon)
Build AIX-compliant wrappers for other AI tools (Gemini, GPT, local models)
---
License
MIT — use it, fork it, build on it, just keep it open.
---
AIX Protocol v1.0 — June 2026
"The web has UX standards. AI deserves the same."
