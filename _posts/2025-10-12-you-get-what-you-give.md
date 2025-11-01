---
layout: post
title: You Get What You Give
subtitle: Mastering AI Prompts for Technical Documentation
tags: [AI, writing]
comments: true
---

AI can draft documentation in seconds, but most prompts produce generic, unusable content. The problem isn't the technology—it's the technique. Technical writers who treat AI as a magic wand instead of a precision tool consistently get disappointing results.

Prompt engineering is emerging as a core professional competency. The difference between "Write documentation for this API" and a well-crafted prompt can mean the difference between an afternoon of rewrites and a solid first draft that sets you on a surer path. Understanding how to guide AI effectively transforms it from a frustrating experiment into a reliable documentation partner.

## How AI Processes Your Prompts

AI language models work by predicting the most probable next word based on patterns in their training data. When you provide a vague prompt, the AI has infinite possible directions to go—so it defaults to the most generic, common response. When you add constraints, specify format, define audience, and assign a role, you're narrowing the prediction space. You're essentially telling the AI which patterns to prioritize.

Think of it like this: a vague prompt creates a huge target area where the AI might land anywhere. Specific constraints shrink that target to exactly where you need the output to be. This is why detailed prompts consistently outperform generic requests—you're reducing ambiguity in the AI's decision-making process.

## Achieving Clarity and Consistency

These prompts help refine language, simplify complex topics, and maintain a consistent voice across documentation.

### Simplifying Jargon

**Prompt:** "Explain the concept of asynchronous data fetching in a way that a first-time user of our software can understand. Use an analogy from daily life to illustrate the process."

**Why This Works:** Defining the audience ("first-time user") and specifying a method ("analogy") controls the output's complexity. The AI retrieves patterns associated with beginner explanations rather than technical deep-dives. The analogy requirement forces concrete, relatable language instead of abstract terminology.
---
layout: post
title: Sample blog post
subtitle: Each post also has a subtitle
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

### Tone and Style Check

**Prompt:** "Review the following paragraph for passive voice, unnecessary jargon, and wordiness. Rewrite it to be concise, use active voice, and maintain a professional, yet friendly tone."

**Why This Works:** Explicit constraints guide the revision process by telling the AI exactly what to look for and change. Multiple constraints work together—"concise" + "active voice" + "professional yet friendly" creates a specific style target. Without these constraints, the AI might focus on only one aspect or miss your intent entirely.

### Consistency Check

**Prompt:** "Act as our style guide checker. Compare the language, capitalization, and formatting in the following two paragraphs. Identify all instances where they deviate from the Microsoft Style Guide standard for technical documents."

**Why This Works:** Assigning a persona ("style guide checker") primes the AI to adopt that role's knowledge base and priorities. Referencing a known standard (Microsoft Style Guide) leverages the AI's training on that specific style system. This combination produces focused, authoritative feedback rather than generic editing suggestions.

## Summarizing and Audience Targeting

These prompts help you repurpose content or ensure your documentation meets the needs of specific readers.

### Executive Summary for Managers

**Prompt:** "Act as a documentation manager. Read the following technical specification and provide a 3-point executive summary focusing only on the key decisions, implementation risks, and required resources."

**Why This Works:** The role specification filters the AI's focus through a manager's perspective. The length limit ("3-point") forces prioritization—the AI must identify only the most critical information. The content focus list ("decisions, risks, resources") explicitly excludes technical implementation details that managers don't need.

### Creating Release Notes

**Prompt:** "Summarize the changes described in the following pull request/bug report logs. Format the output as three reader-friendly bullet points for external release notes for an end-user."

**Why This Works:** Clearly defining the source material (logs) and the transformation needed (technical changes → user-facing benefits) guides the AI's translation work. Specifying "end-user" and "external" signals that internal jargon and technical details should be filtered out. The format constraint ensures consistency across multiple release cycles.

### Generating FAQs

**Prompt:** "Based on the following user manual chapter about 'Installation,' generate five potential Frequently Asked Questions that a new user might ask. Provide a concise, clear answer for each."

**Why This Works:** Asking the AI to anticipate user needs leverages its pattern recognition of common pain points. The source material constraint keeps questions relevant to your actual documentation. Requiring both questions and answers creates a complete, usable FAQ section rather than requiring a second prompt for responses.

## Workflow and Structure Management

These prompts help with structuring documents and breaking down large tasks into manageable components.

### Creating a Document Outline

**Prompt:** "Generate a detailed chapter outline for a new user guide on 'Getting Started with Cloud Deployment.' The outline should include at least five main sections and three subsections for each, covering installation, configuration, and a first project tutorial."

**Why This Works:** Requesting hierarchical structure with specific depth requirements ensures comprehensive coverage. The topic list ("installation, configuration, tutorial") defines the scope while allowing the AI to organize the flow logically. This produces a framework you can iterate on rather than starting from a blank page.

### Step-by-Step Task Breakdown

**Prompt:** "I need to write a procedure for 'Setting up Two-Factor Authentication.' Provide a step-by-step list of the actions, making sure each step begins with a strong action verb and is written as a clear, single sentence."

**Why This Works:** Enforcing stylistic rules (action verb, single sentence) ensures the generated steps adhere to documentation standards and best practices. These constraints also improve clarity—action verbs make steps concrete and executable. The AI understands procedural writing patterns and applies them consistently when given these boundaries.

### Glossary Term Extraction

**Prompt:** "Scan the following technical document. Extract ten key technical terms and provide a one-sentence definition for each, suitable for inclusion in a glossary."

**Why This Works:** The specific number forces prioritization of truly important terms. The format requirement ("one-sentence definition") and usage context ("suitable for glossary") ensure definitions are appropriately scoped—not too brief to be unclear, not so detailed they become mini-articles.

## Anti-Patterns: What Not to Do

Learning from bad examples is just as valuable as studying good ones. Here are common prompting mistakes that produce poor results:

### Vague Requests

**Bad:** "Make this documentation better." **Why It Fails:** "Better" is subjective and provides no direction. The AI doesn't know whether you want simpler language, more detail, different structure, or something else entirely. **Fix:** Specify what aspect needs improvement: "Rewrite this paragraph to use simpler language appropriate for beginners, reducing jargon by at least 50%."

### Missing Context

**Bad:** "Write release notes for the latest update." **Why It Fails:** The AI doesn't know your audience (developers vs. end-users), tone (formal vs. casual), or what information to include. Results will be generic and require heavy editing. **Fix:** "Write end-user-facing release notes for version 2.3. Focus on new features and bug fixes that improve user experience. Use a friendly, non-technical tone. Format as 3-5 bullet points."

### “Kitchen Sink” Prompts

**Bad:** "Explain our API authentication process, create a troubleshooting guide, write example code in three languages, and generate FAQs." **Why It Fails:** Multiple complex requests in one prompt dilute the AI's focus. Each task gets shallow treatment, and the combined output lacks coherence. **Fix:** Break into separate, focused prompts. Complete each task fully before moving to the next, allowing you to refine each component.

### Assuming Context from Previous Conversations

**Bad:** "Now make it more technical." **Why It Fails:** Even in ongoing conversations, pronouns and vague references create ambiguity. The AI might interpret "it" or "more technical" differently than you intend. **Fix:** Be explicit: "Rewrite the authentication section above to include technical implementation details suitable for backend developers, including HTTP headers and status codes."

### No Format Specification

**Bad:** "Summarize this 50-page specification." **Why It Fails:** Without format guidance, you might get a paragraph when you needed bullet points, or a page when you needed three sentences. **Fix:** "Summarize this specification as a one-page executive overview with these sections: Purpose (2 sentences), Key Features (5 bullet points), Technical Requirements (3 bullet points), Timeline (1 sentence)."

## When You're Not Sure Where to Start

What if you know generally what you need but can't articulate the specifics? Use this collaborative meta-prompt to refine your thinking:

**Meta-Prompt:** "Provide an overview of every facet of my request. Determine the points of uncertainty. Ask me questions to help us clarify the prompt."

This turns the AI into a requirements-gathering partner. For example, if you write "I need documentation for our new API," the AI will ask about:

* Target audience (internal developers, external partners, or end-users?)
* Documentation type (reference guide, tutorial, or quick start?)
* Required depth (comprehensive or overview?)
* Format preferences (single page, multi-page, interactive examples?)

With each answer, the AI narrows the scope until you have a precise, actionable prompt. This collaborative approach is especially valuable when you're facing a complex documentation project and need help breaking it down into manageable pieces.

## Conclusion

If you're finding AI tools underwhelming, it's likely not the technology—it's the technique. AI isn't a magical solution; it's a collaborator that requires clear direction. The key to unlocking consistently good results is prompt engineering: the critical skill of guiding the AI with precision.

By planning your request, defining your audience, being explicit about format and constraints, and understanding how AI processes language, you move from simply asking the AI to working with it. The investment in crafting better prompts pays immediate dividends in output quality, reducing your editing time and producing documentation that meets professional standards on the first pass.