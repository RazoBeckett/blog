---
title: "How to git it!"
date: 2025-07-27
description: "Why I use Git, how it saved me once, and why every dev should care."
tags: ["git", "version control", "dotfiles", "developer workflow", "beginner friendly"]
categories: ["development", "tools"]
cover: "cover.webp"
draft: false
---

*Why I use Git, how it saved me once, and why you should care even if you're a solo dev.*

## That one time Git saved my ass
---

Back in my diploma days, I was working on a Python microproject. Everything was going well. I’d written a bunch of code, tested it, cleaned it up — almost done.

And then I did something dumb. I deleted the whole project folder by mistake while clearing up some stuff.

Gone. The entire thing.

But turns out... I had pushed it to GitHub just a day before. So I opened a terminal, cloned it back,

```bash
git clone git@github.com:RazoBeckett/Password-Manager.git
```

and everything was back in place.

That day, I realized Git isn’t just some fancy tool people use on big teams. It’s a personal backup, version history, time machine, and panic button — all in one. If I hadn’t tracked the code with Git and pushed it to GitHub, I’d have lost the entire thing.

## Git — but why?
---

If you’re just using `git add`, `commit`, `push`, and `pull`, that’s honestly enough most of the time.

But here’s why Git becomes a real game-changer once you get into the habit:

- You can try out weird, risky stuff in a separate branch without touching your main code.
- You can go back to previous states of your files like nothing happened.
- You don’t need to zip your folder every time before making changes.
- It gives you freedom to experiment without fear.

Even if you're working solo, Git gives you peace of mind. You stop worrying about breaking stuff because you know you can always roll back.

## I didn’t learn Git from a course
---

When I first started, I wasn’t doing much with Git. It was just `git init`, commit, push. That’s it.

Things changed when I switched to Linux.

On Linux, everything is a config file. I kept tweaking stuff — my terminal, window manager, keybinds, scripts, themes. I needed a way to manage all those files safely and try new setups without losing what worked.

That’s when Git started making sense. I started tracking my [dotfiles](https://github.com/razobeckett/dotfiles), trying different configs, and rolling back easily when something broke.

Later on, I got into open source. I was following [Chris Titus Tech](https://www.youtube.com/@ChrisTitusTech) and ended up contributing to some of his projects like:

[dwm-titus](https://github.com/ChrisTitusTech/dwm-titus/pulls?q=sort%3Aupdated-desc+is%3Apr+author%3Arazobeckett) | [bash-config](https://github.com/ChrisTitusTech/mybash/pulls?q=sort%3Aupdated-desc+is%3Apr+author%3Arazobeckett) | [linutil](https://github.com/ChrisTitusTech/linutil/issues?q=sort%3Aupdated-desc%20is%3Apr%20author%3Arazobeckett)

That’s where I got more comfortable with branches, commits, rebases, PRs, and all that.

But it all started from managing dotfiles and breaking things on my own system.

## What tools do I use?
---

I'm a terminal-first kind of person. I like to keep things simple and fast.

- **Git CLI** – Just the basic `git` command. It does everything I need.
- **[vim-fugitive](https://github.com/tpope/vim-fugitive)** – A plugin for Vim/Neovim. Helps me stage specific hunks, view diffs, write commits — all inside the editor. No switching windows.
- **[LazyGit](https://github.com/jesseduffield/lazygit)** – A TUI app that gives a clean overview of branches, changes, logs. I mostly use it when I want a quick look at the repo status.

I’ve tried stuff like GitKraken and VS Code’s Git UI. They’re fine, but I just found them too clicky. Terminal is faster once you get the hang of it.

## Git ≠ GitHub
---

This still confuses a lot of people early on, so let’s clear it up.

- **Git** is a version control tool. It runs locally. You don’t need internet to use Git.
- **GitHub** is a platform to host your Git repositories and collaborate with others.

You can use Git without ever touching GitHub. But if you want to back things up or share your code, GitHub makes it easy. There are also alternatives like GitLab, Codeberg, and Gitea if you're into self-hosting or privacy.

## Where to start if you’re new
---

Don’t overthink it. You don’t need to “master” Git before you start using it.

- Create a new project and run `git init`.
- Track your code.
- Commit small changes regularly.
- Push it to GitHub, even if it’s private.
- Use it for your notes, config files, scripts — anything you change often.

Check out the [GitHub Git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf) if you want a quick reference.

## Final thoughts
---

You don’t need to know everything about Git to use it.
You just need to know enough to not lose your work — and enough to try something crazy without worrying about messing things up.

Start using Git today. For your projects. For your configs. For peace of mind.

And remember:
**Always push your code.** You never know when you’ll thank yourself later.
