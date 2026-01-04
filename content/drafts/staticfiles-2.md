---
date: '2026-01-03T14:06:55-05:00'
draft: true
title: 'Staticfiles 2'
---
There's a **hidden footgun in Django deployments**.
Here’s a subtle Django bug that only appears *after* you scale.

Manifest static files are great—until you deploy twice.

By default, Django writes **one global `staticfiles.json` manifest**.

In rolling deployments:
• New code updates the manifest
• Old code is still running
• Templates reference files that no longer exist

Result?
💥 Random 500 errors
💥 Missing static assets
💥 Nightmarish debugging

The fix is simple—but undocumented:
👉 Version your manifest by release (Git hash, timestamp, etc.)

Once you do that, rolling deployments stop breaking.

**CTA:**
I included a full implementation for both S3 and local storage in my latest article.
This is one of those things you only learn the hard way—unless someone tells you first.
