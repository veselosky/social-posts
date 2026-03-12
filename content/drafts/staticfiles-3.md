---
date: '2026-01-03T14:13:23-05:00'
draft: true
title: 'Staticfiles 3'
---

## Here's a crash course on Django's staticfiles architecture

Django's staticfiles app overrides the runserver command to serve static assets during development. In production, Django expects some other process to handle static files. At deployment time, you have to run:

manage.py collectstatic

What happens depends on what you configure in your STORAGES setting.

There are two common deployment patterns:

1. **A local web server**
   - STORAGES['staticfiles'] is set to Django's ManifestStaticFilesStorage.
   - collectstatic gathers static files into a single directory.
   - A web server (Nginx/Apache/Caddy/etc.) serves static files from that directory.
   - Web server passes other requests to Django.
2. **S3-style object storage.**
   - STORAGES['staticfiles'] is set to S3ManifestStaticStorage (from the django-storages package).
   - collectstatic uploads static files to S3.

In both cases, it is wise to use a CDN in front of your static file server for performance and reliability. Then set STATIC_URL to point to the CDN URL.

In a future post, we'll talk about why those storage backends have "Manifest" in their names, and why that's critically important.

Stay tuned!
