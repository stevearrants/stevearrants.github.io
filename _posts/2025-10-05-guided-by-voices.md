---
layout: post
title: Guided By Voices
subtitle: Using AI in Technical Writing
tags: [AI, writing]
comments: true
---

AI is now part of our products and workflows. It's here to stay. Management is increasingly advocating for AI tools as a strategy to reduce headcount, support costs, and time to market. This raises challenging questions for technical writers and editors: Should you adopt AI methods and tools, and if so, what are the essential guidelines and guardrails to follow?

### Where We're At

Statistics reveal a dramatic shift: by 2024, 78% of organizations were using AI in at least one business function (McKinsey & Company, 2025). It's clear why. You get faster drafts, shorter cycle times, and consistent formatting.

But what about accuracy? 54% of workers worry that AI outputs are inaccurate (Salesforce, 2024). For technical documentation, where a single error can halt a user's workflow or generate support issues, this is an unacceptable risk.

### What Are Technical Writers Doing with AI?

Writers have found practical, low-risk applications for AI that go beyond the hype (Johnson, T., 2024; Ferri Benedetti, F., 2024). AI is  useful for quick summaries, data formatting, clarifying complex ideas, and catching inconsistencies (MadCap Software, 2024).

### Technical writers use AI for these tasks:

* **Getting Words on the Page:** Handles initial drafts, outlines, and standardized descriptions. Some writers report doubling productivity on this task (Johnson, T., 2024), though remember that actual writing is only about 20% of a tech writer's day.
* **Handling Tedious Tasks:** Shines at generating tables, YAML structures, indexes, and content categorization. Can auto-classify content for structured frameworks (e.g., DITA).
* **Enforcing Consistency:** Brings content contributed by Subject Matter Experts (SMEs) into alignment with style guides, catching terminology drift and style and language violations.
* **Speeding Up Research:** Offers faster retrieval of accurate, current information. Platforms like Google's NotebookLM are also used to generate text, audio, and video overviews and summaries of complex information. (Verification is still mandatory.)
* **Expanding Language Reach:** Accelerates translation workflows by combining machine translation with AI (requires human review for technical and cultural accuracy).
* **Breaking Writer's Block:** Acts as a brainstorming partner by suggesting alternatives when a writer is stuck on a paragraph or conclusion.
* **Migrating Legacy Content:** Analyzes and maps existing documentation to new structured formats, saving weeks of manual work.

### Where AI Stumbles and Falls

While the utility of AI in low-risk applications is clear, the true danger lies in areas demanding absolute precision, such as documenting complex procedures, specialized terminology, APIs, or regulatory content. Trusting this high-stakes content solely to AI is risky because fundamental accuracy issues have not been solved. For instance, even with 81% of developers planning to leverage AI for code documentation (Stack Overflow, 2024), accuracy remains a major concern (Garn, D., 2024).

The core of the problem is the Hallucination Trap. Because AI's training data is often outdated or incomplete, it will confidently invent details—from system requirements and version-specific instructions to command flags. These creations can manifest as subtle errors that are difficult to spot without expertise. A prime example is an AI generating example SQL commands with proper syntax that ultimately fail in production because the model confused NoSQL, PostgreSQL, and MySQL conventions. These critical errors are often only caught when a Subject Matter Expert (SME) tests the actual command.

Alarmingly, the issue of errors isn't necessarily improving with new technology. Recent data suggests that newer models are not inherently more reliable. The latest OpenAI reasoning models, for example, actually hallucinate more on factual questions than their predecessors, with error rates as high as 48% for the o4-mini model (Techopedia, 2025). This rising error rate underscores the ongoing need for rigorous human review in all precision-dependent tasks.

### Don't Skip Verification!

When using AI for technical content, these three verification steps are required:

1. **Treat AI Output as a Draft:** Never allow organizational pressure to turn AI output into finished work (MIT Sloan, 2025). You wouldn't release an unedited or unreviewed draft, would you?
2. **Get Subject Matter Expert (SME) Validation:** Every technical claim, code sample, command, or procedure must be validated by someone who works with the system. This is non-negotiable. At the very least, do procedure testing on each step.
3. **Check Documentation Standards:** Verify consistency against existing content, terminology databases, and style requirements.

#### Watch for these specific problems:

* Function names or parameters that don't exist
* Syntax from outdated versions
* Concepts borrowed from similar but different technologies
* Authoritative statements about nonexistent features

### Legal Considerations You Need to Know

The risks associated with AI-generated technical content extend directly into the legal and compliance sphere. It is important to recognize that liability for technical errors rests squarely with your organization, not the AI vendor. The consequences of inaccurate, published procedures are ultimately owned by you, making internal verification a necessity. Furthermore, the intellectual property landscape remains volatile due to copyright gray zones, as questions regarding the legality of AI training data are unsettled in court. To navigate these issues, organizational policy is key: you must determine your company's stance on AI use, which may range from requiring explicit AI use statements to prohibiting disclosure of certain content entirely. Finally, implementing a robust quality control process is vital: you must document your process by noting which sections used AI, what human verification steps took place, and who ultimately validated the technical accuracy. This documentation supports accountability and defends the quality of your official content.

### Making Human-AI Collaboration Work

The effective model views AI as a drafting assistant, not an author replacement (Fluid Topics, 2025). Your human role expands to become the architect, validator, and quality enforcer.

The process flow that works is *Iteration*, not *automation*:

1. Generate a draft using AI.
2. Validate the output.
3. Regenerate or correct based on validation.
4. Validate again.

### Clear Boundaries: When to Avoid AI

Given the inherent risks of hallucination and the lack of verification in current models, clear boundaries must be established for AI usage. Organizations should avoid using AI for content that requires high precision, institutional context, or covers novel areas. Specifically, AI should not be trusted with documentation regarding Novel or Emerging Technology with no training data, Safety-Critical Procedures where errors can cause physical harm, Legal or Regulatory Content requiring precise and auditable language, or Highly Specialized Domains with limited public documentation. It is also unsuitable for Content requiring institutional context or organizational history, as this information is absent from its general training sets. Fundamentally, AI models are designed to predict *plausible* content; they do not verify *truth*. Over-reliance on them will inevitably erode both the quality of the final output and the critical thinking skills of the human experts responsible for it.

### The Real Trade-offs

AI offers efficiency gains: faster drafting, better consistency, less repetitive work. However, it demands more sophisticated quality control, not less. Technical accuracy verification becomes the sine qua non.

The trade-off is not between time and quality; it is an issue of time qualification: less drafting time means more validation time. The promise of AI content creation only works if you can accept lower accuracy standards. That's often not a smart trade.

### References

> I’ve saved these links over the past year or so for reference and sharing. The links to **Fabrizio Ferri Benedetti** and Tom Johnson should be in your Tech Writing Favorites. I always find something instructive and interesting on their sites.

* AIMultiple (2024). [AI Hallucination: Comparison of the Popular LLMs](https://research.aimultiple.com/ai-hallucination/)
* Ferri Benedetti, F. (2024). [How I'm using AI as a technical writer](https://passo.uno/ai-tech-writer-examples/)
* Fluid Topics (2025). [Will AI Replace Technical Writers?](https://www.fluidtopics.com/blog/industry-trends/will-ai-replace-technical-writers/)
* Garn, D. (2024). [Will AI replace technical writers? One user's experience](https://www.techtarget.com/searchenterpriseai/opinion/Will-AI-replace-technical-writers-One-users-experience)
* Johnson, T. (2024). [AI is accelerating my technical writing output, and other observations](https://idratherbewriting.com/blog/ai-is-accelerating-me)
* Johnson, T. (2024). [My 2024 technical writing trends and predictions](https://idratherbewriting.com/blog/2024-tech-comm-trends-and-predictions)
* MadCap Software (2024). [AI for Technical Writers - Practical Strategies for Better Documentation](https://www.madcapsoftware.com/blog/ai-for-technical-writers/)
* McKinsey & Company (2025). [The State of AI: Global survey](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai)
* MIT Sloan Teaching & Learning Technologies (2025). [When AI Gets It Wrong: Addressing AI Hallucinations and Bias](https://mitsloanedtech.mit.edu/ai/basics/addressing-ai-hallucinations-and-bias/)
* Salesforce (2024). [Generative AI Statistics for 2024](https://www.salesforce.com/news/stories/generative-ai-statistics/)
* Stack Overflow (2024). [2024 Developer Survey: AI](https://survey.stackoverflow.co/2024/ai)
* Techopedia (2025). [48% Error Rate: AI Hallucinations Rise in 2025 Reasoning Systems](https://www.techopedia.com/ai-hallucinations-rise)
* Wikipedia (2025). [Hallucination (artificial intelligence)](https://en.wikipedia.org/wiki/Hallucination_%28artificial_intelligence%29)