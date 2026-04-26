---
layout: post
title: "What You Leave Behind"
subtitle: "A Contract Technical Writer's Guide to End-of-Engagement Transitions."
tags: [contracting, writing]
comments: true
---

You are a context owner. You've spent weeks or months learning a product, its users, its internal language, and its undocumented quirks. You've mapped the territory between what engineering knows and what customers need. That context lives in your head, your notes, and in your muscle memory for navigating a CMS or the Git repo.

When the contract ends — whether planned or abrupt — that context is at risk. What you do in the final days determines whether the company retains it or loses it. And what you do *after* you leave determines whether you're a professional protecting your boundaries or a free help desk.

![what we leave behind](../assets/img/what-we-leave-behind.png)

## The Planned Ending

If you know the end date, you have time to do this right. Start transition work at least two weeks before your last day — earlier if the documentation setup is complex.

### Deliverables to Produce

**Documentation inventory.** A complete list of every document you created or substantially revised, with locations, last-updated dates, and ownership status. If nobody owns a document after you leave, say so explicitly. Orphaned docs rot fast.

**Style and standards reference.** If you established or enforced style decisions — terminology choices, template structures, voice and tone guidelines, tool configurations — capture them in one place. Don't assume anyone else internalized them. They didn't.

**In-progress work log.** Everything that's partially done: drafts, outlines, tickets you were researching, conversations with SMEs that haven't been documented yet. Include enough context that someone can pick up where you stopped without reverse-engineering your notes.

**Access and tooling documentation.** Every system you touched: CMS credentials, repo access, API keys for documentation tools, CI/CD pipeline configurations, publishing workflows. List what needs to be transferred and to whom.

**The runbook** (see below).

### Handoff Meetings

Schedule at least one handoff meeting with whoever will own the docs next — whether that's another writer, a product manager, or an engineer who drew the short straw. Walk through the inventory, the runbook, and the known gaps. Record it if the company allows it.

If there's no clear successor, escalate that in writing. Send an email to your manager documenting that no handoff recipient has been identified. That protects you later when someone asks why the transition was rough.

## The Abrupt Ending

You got laid off. The contract was terminated early. You're told today is your last day.

You still have obligations, but they're limited by what's reasonable in the time you have. Focus on the highest-value items.

**Minimum viable transition:**

1. Documentation inventory — even a rough one exported from your file browser or CMS.
2. A short email listing in-progress work, where files live, and critical access information.
3. The runbook, if you've been maintaining one throughout the engagement (and you should be).

If you're walked out the same day with no transition time, that's the company's decision and its consequence. You are not obligated to reconstruct institutional knowledge from memory after your access is revoked.

## Solo Writer vs. Team

**Solo writer.** You're the entire documentation function. The stakes are higher because there's no one who shares your context. Your runbook and inventory are the *only* continuity mechanism. Be thorough. Assume the next person will start with zero context — because they will.

**Team member.** Your colleagues carry some shared context, but don't overestimate overlap. Document your specific responsibilities, the areas only you touched, and any processes or tools you owned that the team depended on. The risk here isn't total knowledge loss — it's gaps no one notices until something breaks.

## The Runbook: Your Standard Deliverable

A transition runbook isn't a favor. It's a professional deliverable you should produce on every contract engagement. Start building it in your first week and update it as you go.

### Sample Runbook Outline

```
# Documentation Transition Runbook
## [Company Name] — [Your Name] — [Date]

### 1. Documentation Ecosystem Overview
### 2. Content Inventory
### 3. Workflows and Processes
### 4. Style and Standards
### 5. Stakeholder Map
### 6. Known Issues and Gaps
### 7. Tribal Knowledge
```

**Section 1: Documentation Ecosystem Overview.** This is the "how do I even get started" section. List every tool and platform involved in the documentation lifecycle — CMS, Git repos, static site generators, CI/CD pipelines, publishing targets, analytics dashboards. Include access requirements, credential locations (or who manages them), and environment setup instructions. The goal: a new writer should be able to go from zero to functional workstation using this section alone. If setup took you a week of Slack messages and guesswork, document the path you wish you'd had.

**Section 2: Content Inventory.** A complete manifest of what exists, where it lives, and who owns it. Include document titles, file paths or URLs, last-updated dates, and current status (active, draft, deprecated, orphaned). Map the content architecture — how documents relate to each other, what's organized by product vs. audience vs. workflow. List templates, reusable components, and snippet libraries. This section answers the question every successor asks first: "What do we have?"

**Section 3: Workflows and Processes.** Document the content lifecycle from idea to publication. Cover the creation workflow (draft → review → publish), who participates at each stage, and what the expected turnaround times are. Include publishing and deployment steps — especially if they involve build commands, staging environments, or manual steps that aren't obvious. Add any QA checklists, link-checking routines, or validation processes you followed. If the workflow has pain points or bottlenecks, note those too. A successor who inherits the process should also inherit your understanding of where it breaks down.

**Section 4: Style and Standards.** Point to the style guide if one exists. If it doesn't — if the style decisions live in your head — this section *is* the style guide. Document terminology decisions (did the company settle on "workspace" or "environment"?), glossary entries, template usage rules, and voice and tone notes. Include the *reasoning* behind non-obvious decisions. "We use 'workspace' because the API uses that term and customers file support tickets using it" is far more useful than "Use 'workspace.'" The reasoning prevents the next writer from reliably making the same decision without you.

**Section 5: Stakeholder Map.** Who knows what, and who approves what. List key SMEs by name and domain — the engineer who owns the auth module, the PM who can explain the pricing model, the support lead who knows what customers actually complain about. Include review and approval contacts for each content area, and escalation paths for when reviews stall. This section is social infrastructure. It took you time to build these relationships and learn who to ask about what. Don't make the next person start over.

**Section 6: Known Issues and Gaps.** Be honest about what's broken. List documentation debt: pages that are outdated, sections with known inaccuracies, areas where the product has changed but the docs haven't caught up. Include planned work you didn't get to — features documented in tickets but not yet written up, restructuring projects scoped but not started. Note recurring pain points: content that generates repeat support tickets, sections users consistently misunderstand, areas where the product UX and the documentation tell different stories. This section isn't an admission of failure. It's a professional assessment of the work that remains.

**Section 7: Tribal Knowledge.** This is the most valuable section and the hardest to write. It captures everything you know that isn't documented anywhere else. Undocumented processes or workarounds ("the staging build fails silently if you don't clear the cache first"). People-to-topic mappings ("ask Maria about the legacy import format — she's the only one who remembers why it works that way"). Historical context that shapes current decisions ("we stopped using the wiki because of the 2023 migration incident — the content is still there but nobody trusts it"). This is the section most likely to walk out the door with you. It's also the section that makes the difference between a smooth transition and six months of the new writer reinventing your discoveries.

## After You Leave: Free Work, Boundaries, and What They Pay For

This is where most contract writers struggle. The contract ended, but the questions didn't. Someone emails you: "Quick question — where's the template for the API docs?" Then: "Can you review this draft real quick?" Then: "We're having trouble with the publishing pipeline you set up."

### What's reasonable to do for free

- Answer one or two quick factual questions in the first week or two ("The template is in /docs/templates/api-reference.md").
- Point someone to information that's already in the runbook.
- A brief clarifying email if something in your handoff materials is genuinely ambiguous.

### Where to draw the line

Anything that requires you to *produce work* — writing, editing, reviewing, troubleshooting, training — is paid work. The line isn't complicated: **if it takes more than five minutes or requires you to think rather than recall, it's a billable task.**

Some specific examples:

- "Can you review this draft?" — That's editing. It's paid.
- "Can you walk our new writer through the process?" — That's training. It's paid.
- "The pipeline broke, can you fix it?" — That's engineering support. It's paid.
- "Can you write up how you did X?" — That should have been in the runbook. If it wasn't, producing it now is paid.

### Language for the conversation

Keep it professional and direct:

> *"Happy to help — that falls outside the scope of our completed engagement. I'm available at [rate] for post-contract support. Want me to send a short SOW?"*

> *"I covered that in the transition runbook [section/page]. Let me know if something there is unclear."*

> *"For anything beyond quick clarification, I'd need to set up a short-term support agreement. I can send terms if that's useful."*

Don't apologize. Don't over-explain. You're not being difficult — you're being a professional who values their own expertise. The same expertise they hired you for in the first place.

If the company pushes back, remember: they ended the contract. The expectation that your knowledge remains available for free afterward is the expectation that context has no value. You know better.

## The AI Angle: Why "We'll Just Use AI" Is a Trap

Here's where this gets pointed. More companies are terminating writing contracts and shifting to AI-generated documentation. The reasoning sounds clean: the AI can write, we have the source material, we don't need the writer anymore.

It's a trap. And it springs slowly enough that most companies don't realize they're in it until the damage is done.

**AI generates text. It doesn't generate understanding.** An LLM can produce grammatically correct documentation from API specs, code comments, and existing content. What it can't do is decide what to document, for whom, in what order, and at what depth. Those decisions require understanding the audience — not the abstract "user" but the actual people who file support tickets, abandon onboarding flows, and misuse features in predictable ways. That understanding is what you carried as the context owner. When you leave and nobody replaces that function, the AI produces documentation that is technically accurate and practically useless.

**The quality collapse is gradual and invisible.** AI-generated docs don't fail obviously. They fail quietly. The content is plausible. It passes a cursory review. But it doesn't anticipate the user's actual confusion points. It doesn't structure information around real workflows. It doesn't know that the "Advanced Settings" section is where 60% of support tickets originate, so it deserves twice the attention. Six months after the writer leaves, the documentation looks fine on the surface. Support ticket volume is up 30% and nobody connects the two.

**AI can't maintain its own context over time.** Documentation isn't a one-time generation task. It's a living system that needs to respond to product changes, user feedback, and shifting business priorities. Every time the product ships a new feature, someone has to decide where that feature fits in the existing content architecture, what it replaces, what it breaks, and how to communicate the change to users who learned the old way. That's editorial judgment. An AI tool pointed at a changelog will produce a "what's new" page. It won't restructure the getting-started guide because the new feature changes the recommended onboarding path. That restructuring requires context the AI never had.

**AI can't learn from the audience.** A writer reads support tickets, sits in on customer calls, watches where users get stuck during onboarding, and notices patterns in the questions that come in after a release. That feedback loop reshapes the docs over time — you learn that users skip the overview and go straight to the API reference, so you put the critical warning *there* instead of burying it in the getting-started guide. AI has no feedback loop. It generates the same content regardless of whether the last version confused every reader who touched it. The only way AI-generated docs improve is if a human reads the feedback, diagnoses the problem, and rewrites the prompt. That human is doing the writer's job. They're just doing it worse, with an extra layer of indirection.

**The trap closes when they need to change direction.** Companies discover the real cost when they try to do something new with the docs — a major product pivot, a new audience segment, a migration from one platform to another. The AI-generated content has no underlying information architecture, no consistent editorial logic, no documented style rationale. It's a pile of individually acceptable pages with no connective tissue. Restructuring it requires exactly the kind of contextual understanding they eliminated when they cut the writer.

**The cost of rework exceeds the cost of continuity.** Here's the math companies don't do before they cut the writer: rebuilding documentation context from scratch costs more than maintaining it ever did. When they eventually hire someone — contract or full-time — to fix the AI-generated docs, that person will spend weeks or months doing discovery work that the original writer had already completed. They'll reverse-engineer the information architecture, re-interview SMEs, re-learn the audience, and rediscover the tribal knowledge that walked out the door. The company will pay for that context twice. The second time will cost more, because now they're also undoing the damage from the gap.

**Your transition deliverables are your proof of value.** This is why the runbook, the inventory, the style rationale, and the tribal knowledge section matter beyond professional courtesy. They are a concrete record of the judgment layer that sat between the raw product knowledge and the published documentation. They demonstrate that the work you did was never just typing — it was decision-making informed by audience understanding, content strategy, and institutional context.

If you left a good runbook, some of that context survives your departure and gives whoever comes next — human or AI operator — a leg up. If you didn't, they'll email you. And that email is a consulting engagement, not a favor.

The transition deliverables described in this article aren't just about leaving well. They're about making visible the work that companies are most likely to undervalue — and most likely to miss when it's gone.

## Two Things to Do Before You Even Start

**Build transition time into your contract.** Negotiate a clause that allocates your final one to two weeks for transition deliverables — runbook completion, handoff meetings, inventory finalization. If the contract is terminated early, the clause should specify whether transition work is included in the remaining obligation or billed separately. Don't leave this to goodwill. Get it in writing before the engagement begins, when your leverage is highest.

**Protect your portfolio.** Confirm in writing what work samples you can retain for your portfolio. Most contract agreements assign ownership of deliverables to the client, but you can often negotiate the right to use anonymized or redacted samples. Do this at the start of the contract, not on your last day. If the contract is silent on portfolio use, clarify it before you need it. After you leave, getting permission becomes harder — and the person who could grant it may not remember you.
