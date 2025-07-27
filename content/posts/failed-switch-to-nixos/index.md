---
title: "A 538‑Day Love Affair with the Bleeding Edge"
date: 2025-06-24
description: "My Failed Switch to NixOS, or Why I Still Live in Chaos on Arch."
tags: ["nixos", "archlinux", "linux", "os"]
categories: ["linux", "os-experience"]
cover: "cover.webp"
draft: false
---

A 538-Day Love Affair with the Bleeding Edge
--------------------------------------------

I once told someone, "Nix is for stability. I live in organized chaos." I didn't realize how true that was until I tried to leave.

I gave NixOS a real shot. The promises of perfect reproducibility, declarative configurations, and atomic upgrades whispered sweet nothings in my ear. On paper, it's the endgame—a system as a pristine, version-controlled artifact. A **monument**.

But my computer isn't a monument. It’s a **lab**. And in my lab, things explode.

### The Frictionless Playground

An idea strikes at 10 PM. A cool new CLI tool is trending on GitHub. My hands are on the keyboard, and the thought process is simple: _I want to try that. Now._

On Arch, it’s a heartbeat:

    yay -S some-cool-package

Five minutes later, I’m running it. Maybe it’s brilliant. Maybe it’s useless. Ten minutes after that, I’ve satisfied my curiosity, and it’s gone.

    sudo pacman -Rns some-cool-package

It vanishes. No trace, no configuration to roll back, no “generation” to manage. The experiment is over. My system didn’t just allow it; it got out of the way.

This is my workflow. A constant, churning cycle of discovery and destruction. I don't want my system to remember my fleeting whims. I want it to be a blank canvas, ready for the next chaotic splash of paint tomorrow.

With Nix, I pictured that same 10 PM spark of curiosity, but instead of a quick command, I saw myself editing `configuration.nix`, adding a package, and patiently waiting for the system to rebuild itself. The process, designed for ultimate safety, felt like a cage around my curiosity.

### Why Arch Still Feels Like Home

There’s a reason I’ve lasted 538 days on a single Arch install without a reinstall. It’s not because it never breaks. It’s because the philosophy fits me like a glove.

*   **The Bleeding Edge is My Comfort Zone:** I like the thrill of a `pacman -Syu` and seeing hundreds of packages update. It's a direct connection to the living, breathing world of open source.
*   **The AUR is My Candy Shop:** If a piece of software exists and can be compiled, I can try it in minutes. It’s the world’s most exciting, chaotic, and functional repository.
*   **Fixing is the Fun:** The moments I’ve learned the most are when a bad config or a weird update breaks something. I don’t want guardrails. The process of digging in, understanding the problem, and fixing it myself is the whole point. It’s how the system becomes _mine_.

My setup is absurdly simple: `/`, `/home`, and a mount for my Windows partition. My cleanup crew is `pacman -Qdtq`, wiping away orphaned packages. It's a lean, mean, experimental machine.

### A System for Play, Not for Posterity

Let’s be honest about my use case. I’m not running critical infrastructure. I am:

*   Endlessly tweaking my own [Neovim colorscheme (uwunified)](https://github.com/razobeckett/uwunified.nvim).
*   Building a [random Go CLI to update DuckDNS](https://github.com/RazoBeckett/duckdnsupdate) because it sounded fun.
*   Patching [dwm](https://github.com/RazoBeckett/dwm) on a whim to see if I can make the bar look different.
*   configuring my [dotfiles](https://github.com/RazoBeckett/dwm)

NixOS would look at this behavior and, rightly, try to protect me from myself. Arch just holds my beer.

I respect Nix. I admire its engineering. If I managed a fleet of servers or a team of developers where consistency was king, I’d be its biggest champion. But I’m not chasing a perfect, immutable system.

I’m chasing frictionless curiosity.

And for that, Arch Linux is still home.
