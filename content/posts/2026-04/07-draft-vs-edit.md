---
date: '2026-04-07T09:01:38-04:00'
title: 'Draft vs Edit'
---
In creative writing we have a thing called the "shitty first draft".
In software, that's your v0.1, the "proof of concept" spike.
AI tools don't understand this, and I think that's a severe limitation.

New writers often don't realize the first draft is intentionally bad. The real work is done in the edit. Plot holes get fixed. Prose gets cleaned up and beautified. Bad writing becomes good writing through editing. I believe it was Jodi Picoult who said "You can always edit a bad page. You can't edit a blank page." Hence the shitty first draft. (Credit to Anne Lamott for coining the phrase "shitty first draft".)

This is surprisingly true of software too. Quality code is produced in the "editing". Error handling. Refactoring. Edge case handling. Performance optimizations. These tend to be added after the "happy path" functionality, and are necessary to make software robust and useful.

LLMs excel at creating shitty first drafts, both in prose and in code. Where most (all?) AI tools fall short is in the editing. I suspect this is a structural flaw not easily corrected. The AI is trained to predict the next word, not to evaluate the quality of the overall piece. It is specifically designed to generate new content. But in editing, whether prose or code, often the best way to improve the work is to remove content, not add it. In fact, the larger a code base becomes, the more likely it is that you can solve problems by removing code rather than adding it. This is the opposite of what LLMs are designed to do.

I suspect this is why some developers are extremely pro-AI, while other equally smart developers find it useless.

If you have a problem and the solution requires writing a bunch of code, then an LLM can be a huge help. But if you have a problem and the solution requires removing a bunch of code, then an LLM is not going to be helpful at all. In fact, it may even make things worse by suggesting more code to add.

As always, the real value is not the code, it is understanding the problem and navigating to a solution.
