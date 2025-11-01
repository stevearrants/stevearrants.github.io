---
layout: post
title: Help Development Create Clear Messaging
subtitle: Work with development to serve users
tags: [writing, deveopment, partnership]
comments: true
---

In the world of software, services, and applications, the way we communicate with users can either enhance their experience or frustrate them. We must talk to them on their level and not treat them as compilers.

Clear, concise, and transparent messaging isn’t just good; it’s essential for helping our users work efficiently and with less frustration. Whether it’s an informational update about a command’s progress, an error notification explaining what went wrong and how to recover, or text within the interface itself, every message is an opportunity to guide and support the user. The goal is to reduce the time users spend deciphering messages so they can get back to work quickly.

### **The High Cost of Confusion**

Poor messaging is more than just a minor annoyance. It can lead to significant problems:

* **Misunderstandings:** Vague or jargon-filled messages confuse users.
* **Increased Cognitive Load:** Making users decipher cryptic notes wastes their time and mental energy.
* **Errors:** Confusing instructions can lead users to input incorrect data.
* **Higher Support Costs:** Ambiguous messages inevitably lead to more support tickets that could have been avoided.
* **User Frustration:** Ultimately, bad messaging frustrates users, potentially driving them away and leading to anger directed at the company.

Research from Google’s user experience teams has consistently shown that users are more tolerant of issues when they understand the root cause, transparent error messages reduce user frustration, and providing a clear path to resolution significantly improves user satisfaction. These principles are reflected in Google’s current technical communication and error handling best practices. You can explore these guidelines further in their [Technical Writing courses on Error Messages](https://developers.google.com/tech-writing/error-messages).

### **Crafting Messages That Connect: Best Practices**

So, how can we do better? It boils down to putting the user first. A useful hint is to write messages as if you’re explaining the situation to someone non-technical, like your mother—if she can understand it, you’re on the right path.

Here are some key best practices:

1. **Be Clear and Concise.** Use simple, direct language to get straight to the point. Avoid unnecessary jargon and cryptic abbreviations unless they are universally understood.
2. **Be Informative:** Explain *why* something is happening, not just *what*. For errors, clearly state what went wrong and provide specific context (like the action performed or data identifiers involved). Never settle for a vague “An error occurred”.
3. **Be Actionable and User-Friendly:** Tell the user what the next step is. Guide them toward a solution without blaming them for the problem.
4. **Be Consistent:** Maintain a consistent style, tone, terminology, and formatting across all messages. Pay attention to punctuation, capitalization, spelling, and grammar. Use a uniform format.
5. **Focus on Quality:** Make message reviews a standard part of the code review process. Proofread carefully and utilize tools like spell checkers and linters.

### **From Bad to Better: Real-World Examples**

Let’s look at how to improve common messages:

* **Instead of:** “Windows has detected an IP address conflict.” **Try:** “Two devices are using the same network address. Restart your router and devices.” *(Clearer explanation and actionable advice)*
* **Instead of:** ‘DLL file is missing or not found.’ **Try:** ‘A required file is missing. Please reinstall this program.’ *(Explains the implication and provides a clear next step)*
* **Instead of:** ‘Windows cannot access the specified device, path, or file. You may not have the appropriate permissions.’ **Try:** ‘Access denied. Try right-clicking and selecting ‘Run as administrator’.’ *(Offers a potential solution)*

### **Tools to Help**

Ensuring message quality doesn’t have to be manual. Tools can assist:

* **Grammar/Spell Checkers:** Extensions like [Harper for VS Code](https://writewithharper.com/) or the [Code Spell Checker](https://streetsidesoftware.com/vscode-spell-checker/), both for Visual Studio Code, can catch errors in message strings within the code.
* **Style Guides:** [Establish and follow a style guide](https://medium.com/%40theoldtechwriter/creating-your-teams-style-guide-a641b47413a3). If your company doesn’t have one, [Google](https://developers.google.com/style), [Microsoft](https://learn.microsoft.com/en-us/style-guide/welcome/), and [Apple](https://support.apple.com/guide/applestyleguide/welcome/web) offer great guides.

### **The Bottom Line**

Code isn’t just for compilers; sometimes, it speaks directly to your customers. Effective user messaging is fundamental to good design and a positive user experience. By writing clear, informative, and actionable messages, we reduce user frustration, minimize support burdens, and empower people to use our products successfully. Let’s commit to communicating better, one message at a time.
z