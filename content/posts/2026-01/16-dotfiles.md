---
dateCreated: '2026-01-11T07:30:00-05:00'
datePublished: '2026-01-16T07:30:00-05:00'
title: 'Dotfiles'
---
Want to take control of your data but don't know where to start? Dotfiles configure your tools and environment. Maybe start by getting that configuration under control. Version control.

If it’s not:
• versioned
• backed up
• synced across your devices
• documented
• reproducible

then you don’t really own it.

Dotfiles define how you work.
Git gives you ownership over that configuration.

The cleanest pattern I’ve found:
• Keep your dotfiles (but not secrets or keys!) in a Git repo
• Deploy them into $HOME via symlinks (using a tool like GNU Stow)
• Add a README.md to document what each file does
• Automate any setup steps with a bootstrap script

Version control: Solved.
Backup: Solved.
Sync across machines: Solved.
Documentation: Solved.
Reproducible environment: Solved.

Own your platform — starting with your own machine.