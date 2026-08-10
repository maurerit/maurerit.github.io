---
title: "Claude Code Is Interestingly Good but yet not..."
date: 2026-07-02T03:53:22-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: true
---

I've been using Claude Code for about two weeks now, just testing what it can do with its memory, its inherent skills, and with superpowers. I have to say that it’s quite good. I don’t think I need the memory because my workflow is very simple, but it’s kind of nice. Would I compare it to Hermes or my install of OpenClaw’s memory? No way, not even close. But it somehow lets me use some shorthand.

Now, I have customized its prompt so that it knows to use Gitea over GitHub, and somehow it knows where my project lives. I’m not sure if it’s inferring this from the remote in the Git repo or if it stored it in memory. I also haven’t tested it the way I have Hermes with infrastructure work, because I don’t view it as my infrastructure agent like I do Gippity. I’ve found Gippity to be far superior at infrastructure work. Claude built my infrastructure, though, via GitHub Copilot and OpenClaw. OpenClaw remains my go‑to infrastructure harness; I spent a lot of time on that agent’s brain, so it knows where everything is and how to get in.

2026-07-19 Update

Claude Code wasn’t that great; I’ve come to realize that it’s doing A LOT to make Claude useful. Claude, outside of Claude Code, is far inferior to Chat Gippity in the same tool. I feel like Claude needs a ton of context engineering to be less wreckless, whereas Gippity just does things that make sense and is careful about what it does.  Such as eating up secrets...

I’ve switched to using Pi, but I’m in the process of ripping out omo from Opencode and installing Superpowers instead. More accurately, I had Hermes rip out omo and install Superpowers, and I was waiting for the latest feature to be deployed and ready before switching back. I’ve really come to like Superpowers. It was good in Claude Code; I feel like with Gippity and Pi it was even better, so I’m curious how well it’ll work in Opencode. I’m fairly certain these open‑source harnesses aren’t doing much context engineering outside of your AGENTS.md and other various .md files you might point your LLM at. So I think the slightly superior TUI of Opencode will make me happier than Pi has. Pi was fun to customize and play with, for sure. I can see that if it were the first one I picked up, I’d have some loyalty to it, but alas, opencode has been good to me so far.

It’s not that Opencode is completely superior; I don’t want you to think I’m some kind of elitist, but there’s one feature I have to have when interacting with an LLM… and that’s the ability to scroll back **and** respond without my screen flashing, going to the prompt, and losing my spot while reviewing the LLM’s output. Claude Code, Opencode, and the Hermes --tui all do this beautifully, and I haven’t even noticed the issues I’d heard about with Claude Code and its wonky scroll‑back implementation. It’s just worked so far.

So, overall, is Claude Code a good harness? Sure, it’s got some niceties. It’s smooth and quick to boot, has some built‑in safety (maybe a bit too much), and is easy on the eyes with decent text rendering to help you read the document that’s being presented. I don’t like that it hides the “thoughts” of the LLM, though; those are fun to read while you’re waiting on the slot‑machine to spin. I also don’t like the vendor lock‑in that Anthropic is trying to normalize again. Very reminiscent of Apple’s walled garden.