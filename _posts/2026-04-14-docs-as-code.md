---
title: Just Use Docs-as-Code
subtitle: Why plain text, open-source tooling, and version control solve most documentation problems — and why it's the right foundation for AI-assisted workflows
tags: [writing, AI, tools]
comments: true
---

Every so often, a new round of debate surfaces in technical writing communities about which tool to use for documentation. The contenders are familiar: commercial authoring platforms, help authoring tools, component content management systems, and the occasional wiki. The arguments are equally familiar — feature comparisons, pricing tiers, migration stories, vendor promises.

I want to make a different case. Not for a specific tool, but for an approach: docs-as-code. And not because it's trendy, but because when you examine what technical writers actually need — flexibility, sustainability, community support, and control over their own work — docs-as-code consistently delivers.

## What Docs-as-Code Actually Means

The term gets used loosely, so let's be precise. Docs-as-code means treating documentation with the same tools, workflows, and rigor that developers use for software: version control, plain-text markup, automated builds, and review processes. Beyond that, the implementations vary enormously.

Your docs can live in the same repository as your code, in a separate repository managed the same way, or in a standalone system with no accompanying software at all. You might use Markdown, AsciiDoc, DocBook, or reStructuredText. Your static site generator might be MkDocs, Hugo, Sphinx, or Docusaurus. You can publish to a hosted site, an internal portal, a PDF, or all three.

That variability is a feature, not a bug. Docs-as-code adapts to your environment rather than requiring your environment to adapt to it.

## The Case Against Commercial Authoring Tools

Commercial authoring platforms have real strengths. Many offer polished interfaces, structured content support, and publishing pipelines that work well out of the box. I've used them throughout my career and I understand their appeal.

But they carry significant costs that aren't always visible at the start of a contract or a tool evaluation.

**Licensing.** Enterprise documentation platforms are expensive, often per-seat, and priced for organizations that have already committed. For smaller teams, consultants, or companies that need documentation without a dedicated budget line, that cost is prohibitive. We're talking a range of between $800 to $5000 per year. And that's per seat, not for a team.

**Vendor lock-in.** Proprietary formats mean your content lives inside someone else's system. Migrating away is painful, time-consuming, and sometimes imperfect. The longer you stay, the tougher it is to leave.

**Bug cycles and support.** Commercial tools with long product histories often carry bugs that have persisted through multiple major versions. Support cycles for established tools can be slow, and there's limited recourse when a critical issue doesn't meet the vendor's threshold for priority. One commercial package **still** has bugs from 2010.

**Skill portability.** Deep expertise in a proprietary tool is valuable inside organizations that use it, but less transferable everywhere else. Technical writers who build their practice around a platform are building around a vendor relationship. That can be valuable, but it's also limiting.

## Why Docs-as-Code Holds Up

**The open-source community is robust and active.** Tools like <a href="https://www.mkdocs.org/" target="_blank">MkDocs</a>, <a href="https://www.sphinx-doc.org/en/master/" target="_blank">Sphinx</a>, <a href="https://gohugo.io/" target="_blank">Hugo</a>, and <a href="https://asciidoctor.org/" target="_blank">Asciidoctor</a> are maintained by active communities with public issue trackers, responsive maintainers, and extensive ecosystems of plugins and themes. When you hit a problem, you can usually find an answer in documentation, a GitHub issue, or a forum thread — often within hours. When a bug exists, there's a path to getting it fixed that doesn't involve a support ticket and a quarterly release cycle.

**The markup ecosystem is mature and well-supported.** Markdown is ubiquitous — supported natively in <a href="https://github.com/" target="_blank">GitHub</a>, <a href="https://github.com/" target="_blank">GitLab</a>, <a href="https://azure.microsoft.com/en-us/products/devops" target="_blank">Azure DevOps</a>, <a href="https://www.atlassian.com/software/confluence" target="_blank">Confluence</a>, <a href="https://www.notion.com/" target="_blank">Notion</a>, <a href="https://www.intercom.com/" target="_blank">Intercom</a>, and dozens of other platforms. AsciiDoc and Asciidoctor offer more structured, semantically rich markup for teams that need it. <a href="https://docbook.org/" target="_blank">DocBook</a> has decades of history behind it. These are not niche formats. They're legible in any text editor, "diffable" in any version control system, and portable to any destination.

**Your developers already have the infrastructure.** If your organization uses Git, GitHub, GitLab, or Azure DevOps for software development, that infrastructure exists and is already supported internally. Documentation can live in the same environment, use the same review workflows, and benefit from the same integrations — CI/CD pipelines, automated testing, access controls. You're not asking IT to support a new system; you're extending an existing one.

**The "it costs time, not money" objection has a flaw.** One of the most common pushbacks on docs-as-code is that it's only "free" if you don't value your own time — that the learning curve offsets the licensing savings. This is worth taking seriously, but the framing is incomplete. Every tool has a learning curve, including commercial ones. The difference with docs-as-code is that the skills you develop are transferable. Proficiency with Git, Markdown, and a static site generator are assets that travel with you across jobs, clients, and industries. Proficiency with a proprietary platform travels less far.

**It works outside the software industry.** Docs-as-code is sometimes framed as a practice for software companies, and it's true that the approach emerged from software development culture. But the underlying principles such as version control, review workflows, structured markup, and automated publishing apply anywhere documentation needs to be accurate, maintained, and scalable. Healthcare and other regulated documentation, scientific publishing, policy writing, regulatory compliance: teams in all of these areas have adopted docs-as-code workflows successfully.

**AI tools work better with plain text — and that matters.** There is a growing conversation in technical writing communities about AI: whether it replaces writers, whether it can be trusted, whether engaging with it is surrender. I want to address that tension directly, because I think the framing is often wrong.

AI tools are most useful when writers govern them. We're doing our job when we set the context, evaluate output, correct errors, and work to maintain the standards that make documentation trustworthy. That is not a diminished role. It is a different and more demanding one. The question is not *whether* to engage with AI, but *how* to engage with it on your own terms.

Docs-as-code makes that easier in a concrete way. AI tools — whether you are using them for drafting, consistency checking, or automated processing — work significantly better with plain text and structured markup than with proprietary binary formats or tool-specific codes. Markdown and AsciiDoc files are readable, parseable, and processable by AI systems without conversion, without extraction, and without losing structure. A plain-text docs-as-code repository is AI-ready.

That opens up real workflows. I have used Claude Agent Skills to process structured content exports and generate both Excel workbooks and Markdown documentation files directly from source data — work that would have taken hours done manually. Those workflows depend on the content being in formats that AI tools can actually read and work with. Plain text and Markdown make that possible. Proprietary formats often don't.

Choosing docs-as-code means your documentation is well-positioned for AI-assisted workflows. This isn't because you are handing work over to a tool, but because you are in a better position to direct one.

## Starting Simple, Scaling Up

The most basic docs-as-code implementation is a Git repository containing Markdown files. For some teams and some use cases, that's entirely sufficient.

Most teams eventually have requirements beyond that — static assets, image management, versioning, localization, multi-format output, integration with a developer portal or help center. The good news is that you can build incrementally, adding components as your requirements become clear, selecting tools that fit your specific needs rather than inheriting a vendor's assumptions about how documentation should work.

You're not locked into a single framework. You're not paying for capabilities you don't use. And when your requirements change (and you know they will) you have the flexibility to adapt.

## A Different Way to Frame the Choice

Here's an analogy that I find useful. If you ask a developer whether they'd rather write code or use a proprietary drag-and-drop interface to build application logic, most will choose to write code. Not because drag-and-drop is worthless, but because code gives them more control, more flexibility, and less dependence on a vendor's design decisions.

The choice facing technical writers is structurally similar. Docs-as-code offers the same benefits: control, flexibility, portability, and a foundation you own rather than rent.

That doesn't mean it's the right choice for every team or every situation. There are contexts where a commercial tool is the better fit — where the out-of-the-box capabilities align closely enough with the team's needs, and the licensing cost is justified. Those contexts exist and there is nothing wrong with going with them.

But for most teams evaluating their documentation approach, especially those already working in environments with Git infrastructure, developer involvement in documentation, or a need to keep costs manageable, docs-as-code deserves serious consideration. Not because it solves every problem, but because it solves the most common ones in a sustainable, flexible, and cost-effective way.

