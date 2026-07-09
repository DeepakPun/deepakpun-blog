---
title: "Moving My Blog Out of My Microservices Cluster"
description: "Why I chose an isolated Astro app over building a fourth microservice."
pubDate: "Jul 09 2026"
heroImage: "../../assets/default.jpg"
---

### Why Isolation Wins

My core application currently runs three healthy microservices: a UI, an API, and Docs. When thinking about adding a blog, I faced a choice: add a fourth service or isolate it completely.

I chose **Astro hosted on Vercel** for a few simple reasons:

- **Zero Maintenance**: No database upgrades or server patching.
- **Security**: A vulnerability in my public blog content cannot expose my core API.
- **Speed**: It builds to pure, static HTML that loads instantly.

This entire site is compiled from simple Markdown files!
