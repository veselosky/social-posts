---
date: '2026-04-13T09:01:38-04:00'
title: 'Hugo'
---
Hot Take: 99% of websites don't need a front end JavaScript framework.
HOTTER Take: 60% of websites don't need a back end framework either.
Here's my solution.

In the past few weeks I have ported several websites from a dynamic back end framework (Django) to a static site generator (Hugo). There are many hosting solutions available for free for small static sites (GitHub Pages, Netlify, Vercel, Cloudflare Pages/Workers, etc.), so if you need cheap hosting, this is a great path.

I surveyed the SSG landscape, eliminating from contention those I have used before (Jekyll, Pelican, Gatsby). Very quickly, my choices narrowed to two: Astro and Hugo. The deciding factor between them came down to templates. Astro wants you to write templates using JavaScript. Hugo is plain HTML. I'm not a JS guy, so Hugo it is. (If you are a JS person, I highly recommend checking out Astro.)

Things to know about Hugo:

1. Hugo is amazingly fast. Blink and you'll miss it fast. Build your whole site in milliseconds fast. Seriously.
2. Hugo, like most SSGs, reads sources from Markdown files with YAML front matter for metadata. Unlike most SSGs, that's not the only option. Hugo also supports other input formats, including raw HTML (good for me).
3. Hugo is written in Go, so in theory, it's a single binary with no complex setup. In practice, however, the recommended way to integrate themes is with Hugo Modules, which requires you to install the Go programming language (you don't have to use it, it just needs to be available for Hugo to use). Still, simpler setup than many tools.
4. Hugo's templates are written in Hugo's extension of the Go template language, which is not entirely intuitive for non-gophers (though it's pretty easy to pick up).
5. Hugo doesn't come with a default template set. You need to pick a theme to install separately, or create your own.

My take: Hugo is usable for any person who's comfortable writing in Markdown and running commands at the command line. But Hugo really shines as a build engine for developers. Minification for HTML, CSS, and JS is built-in. Image optimization, also built-in. While it lacks default site templates, it has built-in partials for common things like open graph metadata, Google Analytics (but don't do that if you value privacy), and pagination. LLM coding models do a reasonably good job with the template language, though it will need some manual fixes.

I plan to keep working with Hugo and see how far I can push the static site architecture. I believe it can do a lot more than most folks think. 

Do you use static site generators? What are your biggest concerns about the tools or architecture?
