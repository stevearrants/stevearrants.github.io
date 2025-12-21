---
title: All Lost in the AI Supermarket
subtitle: 10 Questions Technical Doc Teams Need to Ask Before Buying AI (But Usually Don't)
tags: [writing, AI, tools]
comments: true
---

Every documentation meeting, conference, or event I've attended in the past two years has featured vendors promising that AI will produce better, faster, and more complete documentation. The impressive demos promise productivity gains of 40%, 60%, and even 80%. The sales teams are earnest and enthusiastic.

And yet, what I’m seeing online on Reddit, LinkedIn, and elsewhere is very different from what I see in teams a few months after they've made the jump. The tool that looked transformative in the demo sits mostly unused. The promised integrations turned out to be more complicated than advertised. The writers who were supposed to be freed from documentation scutwork instead spend hours cleaning up and verifying AI-generated content that doesn't *quite* match the product.

After forty years in technical writing and adapting to changes like desktop publishing, the web, and AI, I've found the most important questions aren't answered by vendors during sales calls. They're the questions teams often gloss over or forget to ask themselves before they ever pick up the phone.

Here are ten of them, split between the hard internal conversations you need to have first, and the vendor questions that will tell you whether a tool will work for you.

As you begin your evaluation, here are some AI product categories worth exploring:

-   **Governance** (<a href="https://www.acrolinx.com/" target="_blank">Acrolinx</a>, <a href="https://writer.com/guides/agentic-ai-governance/" target="_blank">Writer</a>): Enforcing strict terminology and style guides.
-   **Hosting/CMS** (<a href="https://document360.com/" target="_blank">Document360</a>, <a href="https://www.gitbook.com/" target="_blank">GitBook</a>, <a href="https://www.intercom.com/" target="_blank">Intercom</a>): Serving content to users via semantic search/chat.
-   **API Docs** (<a href="https://apidog.com/api-doc/" target="_blank">Apidog</a>, <a href="https://www.mintlify.com/" target="_blank">Mintlify</a>): Auto-generating reference docs from code.
-   **Video/Media** (<a href="https://www.techsmith.com/camtasia/audiate/" target="_blank">Camtasia/Audiate</a>, <a href="https://www.guidde.com/" target="_blank">Guidde</a>): Rapid creation of video tutorials and scripts.

**NOTE:** <a href="https://docs.google.com/spreadsheets/d/16xdja02MlVQ5IB9cAmK5uSqaPdZbkDNF8DnfEMGgux8/edit?usp=sharing" target="_blank">Download a checklist in Google Sheet format.</a>.
# Part One: The Internal Reckoning

Before scheduling a single demo, have some honest conversations with your team and stakeholders. These aren't fun, but they'll save you from expensive mistakes.

## 1. What problem are we actually trying to solve?

"We need AI,” "we need to be more efficient," or "leadership wants us to innovate" are not problem statements; they’re undefined goals.

A real problem statement looks like this: "Our SMEs and Project Management are bottlenecked. They spend 30% of their review time fixing basic terminology inconsistencies." Or: "We're publishing 10 new documents a week, and each one takes two hours to write from scratch." Or: "Support tickets about webhooks increased 40% after we shipped incomplete documentation."

I worked on a team last year that bought an AI writing assistant after the engineering VP saw a demo at a conference. Six months later, we’d barely used it. When we dug into why, it turned out their real problem wasn't writing speed—it was that their SMEs couldn’t make time for reviews and didn’t want to learn another tool to review documents. No AI tool was going to fix that. They needed a process change and executive buy-in, not software.

> **Write down your actual problems. Be specific. If you can't articulate what you're solving, you can't evaluate whether any tool solves it.**

## 2. What does our content actually look like?

AI tools can perform very differently depending on the content type. A tool that's excellent at generating first drafts of conceptual overviews might be terrible at API reference documentation. A tool that handles troubleshooting guides well might hallucinate wildly when asked to write about configuration parameters.

Before you evaluate any tool, audit your content. A friend’s company that creates development tools bought an AI tool after seeing it generate beautiful marketing-style content. The documentation team writes integration documentation for enterprise software. The tool's breezy, conversational style was completely wrong for their audience of senior developers who wanted precise technical specifications. The mismatch was apparent in retrospect, but nobody had thought to test with their actual content types.
> **What percentage is procedural versus conceptual? How much is API reference versus user guides? Do you have release notes, knowledge base articles, in-app help, or training materials? What's the technical complexity level?**

## 3. Who will own this, and do they have time?

AI tools require feeding, tuning, and oversight. Someone needs to configure and test the style guidelines. Someone needs to train the team. Someone needs to monitor the output quality. And someone needs to update the tool when the terminology changes and when the product evolves.

If your answer is "we'll figure it out later" or "everyone will pitch in," I can predict your outcome: Intense and enthusiastic use for two weeks, sporadic muttering and frustration for a month, and then the tool is sent to the software graveyard. I've seen this pattern repeat more than once with new tools and technologies.

> **Assign an owner before you buy. Make sure they have actual bandwidth and not aspirational bandwidth. Give them real hours carved out of their existing workload. If you can't make that commitment, you're not ready for the tool.**

## 4. What's our actual risk tolerance for errors?

AI-generated content will contain errors. Not occasionally, but reliably. The question isn't whether you'll need human review, but how much and how rigorous it will be.

Healthcare documentation has different stakes than an SaaS knowledge base. Financial services compliance content is different from a startup's getting-started guide. API documentation that warns of a wrong parameter that could cause data loss is different from a blog post about product philosophy.

Have an honest conversation about your tolerance for error.
> **What happens if incorrect information reaches your users? Who is liable? What's the reputational cost? Then design your review workflow *before* you buy the tool, not after. If the required review process is so extensive that it eliminates the time savings, it’s best to know that upfront.**

## 5. How will we measure success?

"It feels faster" isn't a metric. Neither is "the team seems to like it." If you can't measure the impact, you can't justify the expense—and you can't identify when the tool isn't delivering.

Before you buy, establish baseline measurements: 
> **Time from outline to published draft. Number of review cycles per document. Support ticket volume for documentation-related issues. Writer satisfaction scores.**

Whatever matters to your organization is what you should measure.

Then define what success looks like in concrete terms. A 25% reduction in first-draft creation time? A 15% decrease in SME review cycles? Fifty fewer support tickets per quarter on topics covered by AI-assisted documentation?

Without baseline measurements and clear targets, you don't know where you're going. You'll have no way to prove ROI to skeptical executives or to identify when you need to change course.

# Part Two: The Vendor Conversation

Once you've done the internal work, you're ready to talk to vendors. But skip standard, scripted demos—you need answers that sales presentations are frankly designed to avoid.

## 6. How does your tool handle our specific content types?

Don't accept generic demos with generic content. They're almost always useless. Bring your own real-world samples&mdash;especially the edge cases that make your documentation authoring challenging.

Ask them to process a document with conditional text. Feed it content with strict terminology requirements and see if it maintains consistency. Give it a procedure with twenty steps and see if it preserves accuracy. Test it with your cross-referenced topics and see if it handles dependencies correctly.

The tool that wins in a controlled demo might stumble badly with your actual content complexity. Better to find out before you sign the contract!

## 7. What does the tool actually do versus what does it technically enable?

"AI-powered" can mean anything from a thin wrapper around a general LLM API to sophisticated fine-tuning on technical documentation. The difference really matters!

Ask directly: *"Is this a custom model trained on technical content, or is it calling Claude or GPT-5 with some prompt engineering?" "What documentation-specific training has the model received?" "How does it handle domain terminology that wouldn't appear in general training data?"*

There's nothing fundamentally wrong with a well-designed wrapper around a general model, but you should know what you're buying. A tool that's essentially a ChatGPT interface with documentation prompts might not be worth the premium over creating prompts yourself and using the API directly.

## 8. How does this integrate with our actual toolchain?

"We have an API" is not an integration. "We support all major platforms" is marketing, not technical documentation.

Get specific. 
> **If you're using a docs-as-code workflow with Markdown in Git repositories, how exactly does the tool interact with that? If you're in MadCap Flare or Paligo, what does the integration actually look like? Does it work with your CI/CD pipeline? Your review workflow? Your publishing system?**

Ask for customer references using a similar stack&mdash;then actually call them. Ask what the integration really involved: 
> **How long did setup take? What unexpected complications arose? What workarounds did they have to build?**

## 9. What happens to our content?

This question has three parts, and you need clear answers to all of them.

1. **Is our content used to train your models?** If you're documenting proprietary systems, you probably don't want your integration specifications to improve the AI's ability to later be used to describe your competitors' products.
2. **Where is our content stored, and for how long?** This matters for compliance, for IP protection, and for basic security hygiene.
3. **Who has access to our content? Can the vendor's employees see it? What about their subcontractors?** Get specifics, get them in writing, and have your legal team review them.


## 10. What does "ongoing costs" really mean?

The first price you see is almost never what you’ll actually pay. Enterprise tools have complicated pricing that can lead to unexpected costs as your usage grows.

Get explicit answers: 
> **Is pricing per-seat, per-token, per-project, or some combination? What happens when your content volume doubles? What if you add three writers to the team? Are there usage caps, and what happens when you hit them?**

Ask to cost out specific scenarios. 
> **"What would we pay if we processed 500 documents per month instead of 100?" "What if we need to regenerate content after a major product update?" "What's the cost impact of adding a second product line?"**

Get the real numbers, not the entry-level pricing that gets you in the door. You want to avoid sticker shock!

## The Opportunity Is Real—If You're Prepared

None of this is an argument against AI tools for documentation. I use them regularly, and they've genuinely improved my workflow. They’ve helped me create Python scripts to transfer content between MadCap Flare and Intercom, generate ALT-TEXT for images, and check document sets for inconsistencies. The technology is powerful and getting more capable every month. But is isn't perfect and you can't just give it a document and publish it immediately. 

Powerful tools require thoughtful and well-planned adoption. The teams that get the most value from AI documentation tools are the ones that did the hard work first: understanding their actual problems, auditing their content, assigning ownership, establishing metrics, and asking vendors the uncomfortable questions.

The teams that struggle are the ones that bought the demo.

I've been through enough technological transitions to know that the survivors aren't the ones who adopt *fastest*. They're the ones who adopt *smartest*. It’s no different with AI tools. Do the preparation, ask the hard questions, and you'll be positioned to achieve better productivity with these tools rather than waste budget on shelfware and waste your valuable time.

Your future self—and your documentation budget—will thank you.

> _**Disclaimer** I used AI to check spelling, grammar, and style. It also suggested reorganization in some sections and additional resources to consider, and the illustration to use._
