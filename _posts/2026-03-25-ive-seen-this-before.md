---
layout: post
title: "I've Seen This Before: What Five Technology Transitions Tell Decision-Makers About AI and Documentation"
subtitle: "The pattern is clear. The question is whether you'll repeat the expensive mistake."
---

## You've Heard This Pitch Before

If you manage a product team, run a documentation group, or make budget decisions about content and support, you have been told more than once in the past year that AI is going to transform your documentation. Faster output! Lower costs! Maybe fewer writers?

You should know that I have heard exactly this pitch. I started my career writing documentation on an IBM Selectric typewriter. I have worked through every major shift in documentation technology since: typewriters to word processors, print manuals to online help, desktop help systems to the web and content management, and now into AI-assisted workflows. Each of those transitions came with the same promise to leadership. Each time, the promise was half-right. And each time, the half that was wrong cost organizations more than they expected.

After four decades and so many transitions, the pattern is clear enough to be useful to anyone making decisions about documentation tooling and staffing right now. This isn't a history lesson. It's a diagnostic.

## The Pattern

Every documentation technology transition follows the same three-beat cycle.

First, the new technology automates the mechanical layer of the writer's current job. Word processors eliminated WhiteOut and retyping. Online help tools eliminated pagination and indexing. Content management systems eliminated manual publishing and added content reuse. Each one was a genuine productivity gain, and the organizations that adopted them early benefited.

Second, leadership assumes the writer's role has shrunk. The reasoning feels sound: if the tool does part of the job, you need less of the person. Budgets get cut. Headcount gets reduced. The remaining writers are asked to do more with less, on the theory that the tool makes up the difference.

Third, and this is where the money gets lost, the writer's role has actually shifted upward. The mechanical work is gone, but a new layer of complexity has taken its place, and it requires judgment.

When word processors replaced typewriters, writers weren't just typing faster. They were controlling document structure, managing revision workflows, and making editorial decisions in real time that used to be locked in by the cost of retyping. When print manuals gave way to online help, writers weren't just converting pages to screens. They were designing information architectures of topic-based, searchable, context-sensitive systems that required a fundamentally different way of *thinking* about content. When desktop help moved to the web and content management systems, writers weren't just posting pages. They were managing living documentation systems that had to be updated, versioned, measured, and governed across multiple channels.

At every stage, the organizations that recognized the shift early, that understood the writer's role had become more complex, not less, maintained higher content quality at lower long-term cost. The organizations that treated the transition as a cost-cutting opportunity got what they paid for: content that degraded silently until the consequences showed up in support tickets, onboarding failures, and customer churn.

## Where AI Fits the Pattern — and Where It Breaks It

AI follows the pattern cleanly up to a point. It automates the mechanical layer of the writer's current job with real effectiveness. First drafts, boilerplate content, format conversions, consistency checking, bulk restructuring — these are genuine productivity gains. A skilled writer using AI tools can produce clean, standards-compliant documentation significantly faster than the same writer without them. That part of the promise is real.

The pattern holds on the organizational response, too. The pitch to leadership is familiar: AI can produce documentation, so you need fewer people producing documentation. The logic feels sound. It is the same logic that felt sound in 1984, 1990, in 2005, and in 2010.

Here is where AI breaks the pattern in a way that should concern decision-makers more, not less.

In every previous transition, the output of the new tool was obviously incomplete without a writer's involvement. A word processor produced a blank page. An online help tool produced an empty structure. A CMS produced an unpopulated template. Clearly, the tool was a means of production and not a source of content. Nobody looked at an empty MadCap Flare project and concluded that the documentation was done.

AI is different. AI produces output that looks finished. It is fluent, grammatically correct, well-organized, and formatted appropriately for the context. It *looks* like documentation. It *reads* like documentation. And in many cases, it is wrong — subtly, confidently, and in ways that are difficult to catch without specific domain knowledge.

This is the break in the pattern, and it inverts the risk profile for decision-makers. In previous transitions, the cost of not having a writer was obvious: you had no content. With AI, the cost of not having a writer is hidden: you have content that appears complete but contains inaccuracies, inconsistencies, and structural problems that compound over time. No one notices until support costs climb, until customers complain and flame that the documentation contradicts the product, or until a new hire's onboarding stalls because the setup guide skipped a step that the AI didn't know about.

The cost of bad documentation has always been real. AI has made it insidious.

## The Role You Actually Need

Every transition I have worked through taught the same lesson: when the tool changes, the writer's value moves up one level of abstraction. The mechanical work gets automated. The judgment work gets more important.

With AI, the writer's role moves to what I call context ownership. This is not a soft concept. A context owner is the person in your organization who governs what your AI tools know, how your content is structured, whether the output meets your quality and accuracy standards, and how your documentation systems connect to your product and engineering workflows.

In practice, context ownership looks like this:

A context owner defines and maintains the templates, standards, and structural rules that AI tools follow. Without these, AI produces content that is internally consistent within a single document but inconsistent across your documentation as a whole. Your customers notice, even if you don't.

A context owner reviews and validates AI-generated drafts against product reality. AI tools do not know what your product actually does in edge cases. They do not know what changed in the last release that hasn't been documented yet. They do not know that the API endpoint described in the engineering spec was modified during implementation. The context owner does.

A context owner manages the documentation pipeline. In a modern documentation operation, this means version control, docs-as-code workflows, API-driven publishing, and automated quality checks. These are technical systems that require technical management. AI can operate within these systems, but it cannot design, maintain, or troubleshoot them.

A context owner bridges engineering and customer-facing content. This is the function that has never been automated in any transition, and AI has not changed that. Someone has to understand what engineering built, determine what customers need to know about it, and make sure the documentation connects those two realities accurately. AI cannot attend your sprint reviews. It cannot ask your engineers clarifying questions. It just cannot determine that the feature described in the ticket is not the feature that shipped.

This is not a diminished version of the writer's role. It is a more senior, more technical role than "writer" has traditionally implied. And it is the role that determines whether your AI investment in documentation produces a return or produces a cleanup project.

## What Happens Without a Context Owner

If you're considering whether you need this role, consider what happens without it.

Without a context owner, AI-generated content drifts. Each piece is produced independently, and over time your documentation develops contradictions, duplicated explanations that don't agree with each other, and structural inconsistencies that make content harder to find and harder to trust.

Without a context owner, your AI tools train on their own output. If inaccurate content gets published and then ingested as source material for future AI-generated drafts, the errors compound. The system doesn't self-correct. It self-reinforces.

Without a context owner, no one is accountable for documentation quality. AI is a tool, not a replacement for a human writer. When a customer reports that the documentation is wrong, someone has to own the investigation, the fix, and the system change that prevents it from happening again. That someone needs domain knowledge, editorial judgment, and the authority to make structural decisions about your content.

I have watched organizations go through this cycle with every previous technology transition. The pattern is consistent: the cost of cutting the person who understands the context always shows up sooner or later. It shows up in support costs, in customer satisfaction scores, and in the expensive remediation project that follows when leadership finally acknowledges the problem.

## The Decision in Front of You

You are not choosing between writers and AI. You are choosing between governed AI-assisted documentation and ungoverned AI output.

Governed means a skilled writer sets the structure, defines the standards, manages the tools, validates the output, and maintains the system. AI handles the volume and the mechanical work. Quality stays high. Costs come down over time because the system is designed to scale.

Ungoverned means AI produces content faster than anyone reviews it. Quality degrades silently. The cost shows up later in support escalations, in customer churn, and in engineering time spent answering questions that the documentation should have handled. 

The writers who have survived these technology transitions are not people who resisted new tools. They are people who understood what the tools could and could not do, and who adapted their role to meet the new complexity. They are, in fact, the people best positioned to govern AI-assisted documentation, because they have done exactly this kind of work before with different tools, at a different level of abstraction, under the same fundamental conditions.

## The Lesson from Every Previous Transition

Every time the tool changed, the organizations that invested in the person who understood the context came out ahead. The organizations that treated the transition as a headcount reduction came out behind, and most of them eventually hired their way back to where they started — at greater expense, with lost institutional knowledge, and after a period of content quality that cost them more than they saved.

Our tools are changing again, but he pattern is the same. Be sure you recognize it this time or you'll learn it again the hard way.
