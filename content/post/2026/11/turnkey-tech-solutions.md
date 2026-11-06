---
title: "Turnkey Tech Solutions"
date: 2026-11-05T06:46:14-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: true
---

I get it, we all just want something to work.  Dots from OpenAI (if it works), Grokbot from SpaceXAI, Claude Duet and then maybe Kimi has one as well and also the Deepseek harness might have some kind of swarm?  There's a few free ones that bind up to some various LLM providers.  I've tried [Paperclip](https://paperclip.ing) which almost worked.  But I didn't like it right off the bat because my data is in Gitea... so I got to thinking, let's shim MY systems together.

So the agent-shim was born (not opensource yet) and we're working on a 1.x.x release.  It'll bind up Gitea, PostgreSQL for tracking and RabbitMQ for dispatching.  It will run in 2 parts, the web api which can run anywhere, then a route service which can run off the agent box and then a dispatch service which has to run on host as it is the full tracker and runner of the agents.

So far we have an openclaw connector and are starting to dogfood it a bit.  It fumbled through getting the pi connector working but it managed well.  I can't believe it's been three weeks now.  We've been running tickets through first with just me trying to move them one at a time while we worked towards a working workflow implementation and then with claude assisting the workflow engine until where we are now where I'm hoping to get our first ticket from Spec -> Mergable software.  That way I can start working on the merging and resolving workflow so we can get from Spec -> Built software, and FINALLY, a deploy pipeline.

So, instead of buying totally into one of these providers ways of interacting with their agents and swarms I'm trying to build something fairly specialized to fit my needs.  Ideally one of these days I can afford some local AI but alas, I do subscribe for my brains of the operation.  Which means it could all melt down soon but we'll see.

Onto some specifics.  What we currently have is - An OpenClaw connector, Pi Connector, Workflow engine and dispatch from Gitea.  The shim knows how to interact with Gitea only but we do have plans to interact with Forgejo as well after 1.0.0.  The Pi connector is built with I think 3 different parts.  First we have a small little controller that can spawn sidecars for the builder and also acts as a proxy as well for it's tools like npm and go get.  Whitelists across the board.  We'll reveal even more once the first milestone is reached.  I'm aiming for a fairly seamless install with assistance from an agent.  Sorry people, this is all AI here, documentation will read like a robot built it.

I chose to have an OpenClaw connector because I just haven't migrated my first agents completely off of the harness because I haven't found a memory system as good as OpenClaws plus what else I've slapped in there.  We do have plans for a Hermes connector but I'm focused on the workflow and getting that done first.  So interaction with my first agents is still through OpenClaw.  I do believe though that I will migrate my 'senior agents' off of OpenClaw and onto either pi with [gentle engram](https://github.com/Gentleman-Programming/engram) or Hermes and we'll shim in gentle-engram for some extra memory retention.  I want the memory system because my hope is that they catalog things themselves for later recall to help keep from drifting.

So far, the interactions are including me spending more time in spec mode, killing efforts that went wrong more and using what we can out of that effort in the new redesign.  And I can focus more on the application and testing it to help feed the machine to make it better.  I hope to have a stable product fairly soon so I can put it to use with [mop](https://mop.vapor-sea.space) and see how much more hands off I can become.

As a side note, speaking of mop, I may have to find a new way to host this for the corp so that my work with my agents doesn't disturb their work.  Maybe I go down to one builder and tweak my prompts so that agents know to sleep and monitor a build before reviewing or continuing.  We'll see, the shim is become very flexible already.

I think I'll stop rambling now and say - I get it now why people said to put their agents in a loop... I'm finally building my loop and hope to share it soon.