---
date: '2025-11-08T11:51:04-05:00'
draft: true
title: 'Hugo Pagefind'
---

### 🔎 Adding Search to a Static Site with Hugo + Pagefind

When I relaunched **Control-Escape** as a Hugo-generated static site, I faced a classic problem:

> “How do you add *search* to a site that has no backend?”

Static sites are fast, secure, and simple—but without a server, traditional search just doesn’t work.

That’s where **[Pagefind](https://pagefind.app)** comes in.

🔍 **What it does:**
Pagefind builds a search index *at build time* and ships it with your site.
Then, when a visitor searches, everything happens **in the browser**—fast, lightweight, and privacy-friendly.

💡 **Why I love it:**

* Dead simple to integrate with Hugo (literally 3 steps).
* Compact, lazy-loaded index = minimal performance impact.
* Accessible out of the box (keyboard + screen reader friendly).
* Easy to customize what gets indexed—so outdated or irrelevant pages stay hidden.

Here’s how easy the workflow is:

```bash
hugo build
npx pagefind --site public/
hugo server
```

…and you’ve got full-text search running locally, no external service required.

⚙️ **Pro tip:**
Use `data-pagefind-body` to control which parts of your content get indexed.
I even exclude “outdated” posts automatically with a single Hugo conditional.

---

Static doesn’t have to mean feature-poor.
With tools like Pagefind, **you can have a fast, secure site *and* a modern user experience.**

If you’re running a Hugo site (or thinking about it), give Pagefind a try — you might be surprised how capable “just HTML” can be.

#Hugo #WebDevelopment #StaticSites #Pagefind #Accessibility #WebPerformance
