---
title: "Claude Code Is Interestingly Good but yet not..."
date: 2026-07-02T03:53:22-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: false
---

I've been using claude code for about 2 weeks now.  Just testing what it can do with it's memory, it's inherit skills, with superpowers and I have to say that it's quite good.  I don't know that I need the memory because my workflow is really simple but it's kind of nice.  Would I compare it to hermes or my install of openclaws's memory?  No way, not even close.  But it somehow let's me use some short hand.

Now, I have customized it's prompt so that it knows to use gitea over github and somehow it knows where my project lives.  Not sure if it's inferring it from the remote in the git repo or if it stored it in memory.  I also haven't tested it like i have hermes with infrastructure stuff because I don't view it as my infrastructure agent like I do gippity.  I've found gippity to be far superior at infrastructure work.  Claude built my infrastructure though but through github copilot and openclaw.  Openclaw remains my goto infrastructure harness, spent a lot of time on that agents brain so he knows where everything is and how to get in.

2026-07-19 Update

Claude code wasn't that great, I've come to realize that it's doing A LOT to make claude useful.  Claude outside of claude code is far inferior to chat gippity in the same tool.  I feel like Claude needs a TON of context engineering to make it useful where as gippity just does things that make sense and is careful about what it does.

I've switched to using pi but am in the process of ripping out omo from opencode and installing superpowers instead or more accurately, I had hermes rip out omo and install superpowers and was waiting on getting this latest feature deployed and ready before switching back.  I've really come to like superpowers.  It was good in claude code, I feel like with gippity and pi it was even better so I'm curious how well it'll work in opencode.  Fairly certain these opensource harnesses aren't doing much context engineering outside of your AGENTS.md and other various md files you might point your LLM at.  So I think the slightly superior tui of opencode will make me happier than PI has.  But pi was fun to customize and play in for sure.  I can see if it were the first one I picked up that I'd have some loyalty to it but alas, opencode was my first harness and I think I'll stick with it.

It's not that opencode is completely superior, I don't want you to think I'm some kind of elitist or something but there's one feature I have to have when interacting with an LLM... and that's the ability to scroll back AND respond without my screen flashing and going to the prompt and losing my spot while reviewing the LLM's output.  Claude code, opencode and the hermes --tui all do this beatifully and I haven't even noticed what I'd heard about with claude code and it's wonky scrollback impl.  It's just worked so far.

So, overall, is claude code a good harness?  Sure, it's got some niceties about it.  It's smooth and quick to boot, has some built in safety (maybe a bit too much) and is easy enough on the eyes with decent text rendering to help you read the document that's being presented in front of you.  I don't like that it hides the 'thoughts' of the LLM though, those are fun to read while you're waiting on the slot machine to spin.  I don't like the vendor lockin that Anthropic is trying to normalize again.  Very remiscent of Apple's walled garden.