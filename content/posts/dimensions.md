+++
title = "Dimensions: A Terminal Tab Manager"
date = "2026-01-02T17:18:11-05:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "Karl Muller"
cover = ""
tags = ["dev-tools", "terminal", "configuration", "tmux"]
keywords = ["Dimensions", "tmux", "TUI", "terminal", "Rust"]
description = "An interactive terminal tool that keeps tmux tabs organized into focused workspaces."
showFullContent = false
readingTime = false
hideComments = false
draft = false
+++

I built Dimensions because I kept losing momentum and navigability when working on multiple projects at once. Each project needs it own mix of tabs and switching between them with multiple projects starts to become a pain. Especially with so many new AI CLI tools alongside your running servers and editor, my terminal started to become a juggling act. Dimensions wraps tmux with a fast, visual TUI that keeps my workflows organized as named dimensions so you can move between projects and contexts much easier.

![Dimensions Screenshot](https://github.com/user-attachments/assets/1e1b98ad-1e43-4156-9767-d1b2b212e1cf)

What it does well:

- Group tabs into named dimensions and switch contexts instantly
- Keep processes alive in the background when you swap dimensions
- Fuzzy search across dimensions and tabs for quick navigation
- Persist dimension names, tabs, and commands to disk
- Launch as a tmux popup with a single keybind

If you want to try it, the project lives here: [Dimensions on GitHub](https://github.com/KarlVM12/Dimensions). It is written in Rust with ratatui and leans on tmux for session management.

Quick install:

```bash
curl -fsSL https://raw.githubusercontent.com/KarlVM12/Dimensions/master/install.sh | sh
```

And if you want the popup workflow, add this to `~/.tmux.conf`:

```bash
bind -n C-g display-popup -E -w 80% -h 80% "dimensions"
```

If you do give it a shot, I would love to hear what you want to see next.
