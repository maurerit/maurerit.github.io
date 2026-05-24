---
title: "Optimizing My Usage"
date: 2026-05-06T21:20:32-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: false
---

Last post I 'bragged' about spending only 2.89 or so on GLM-5.1... well... I've optimized that down quite a bit.  You see, I wasn't fully aware of how opencode works with the explore 'task' specifically.  After doing more work with opencode go I was analyzing my usage and I noticed a crap ton of deepseek v4 pro executions and I'm like... I didn't execute all of that, what's going on?  Then it struck me... as I was reading through documentation I noticed they called out this 'explore' agent and I connected that with the explore 'task' and then realized... The explore task used GLM-5.1 to merely 'grep code'...  that's a pretty lightweight task for one of the more expensive openweight models...

So I searched about how to customize that agent.  I'd already done a few things to built in agents permissions so I knew I could affect it in some way but I wasn't sure if I could hard control it's model.  So I set the model to deepseek v4 flash and then implemented another feature with GLM-5.1 and afterwards looked at my usage.  Nearly half of what the prior feature was and I saw a ton of flash executions in the midst of the glm executions so I knew I did it right.  Not only will these explorations be faster but they'll be super cheap so I can potentially assign my coding to kimi k2.5 and turn it into my Sonnet.

I'm trying to come up with a use for Deepseek.  The model is _ok_ and it's quirky.  It's like a junior dev who's fresh out of college and having graduated with a C average.  It can technically do the work but it's code can be ugly as all get out.  For instance, it went nested function crazy in it's first feature.  Then it also created an anonymous stuct inside a function call in multiple places... for the same type... I don't know idiomatic go but that doesn't feel like what an experienced go developer would accept as good go code.

I've also been trying to figure out how much electricity I'm using.  So I was looking at my electricity bill and also a typical task I run with an LLM.  Typically my executions are around 20 minutes or less, never really had one go longer.  So, for each one of those, if the GPU I'm using is a 600w gpu (I believe the top ends are now 900w?) then each of my tasks cost someone an electricity bill of somewhere along the lines of a few cents.  When the model I'm using would bill out at around 30 cents or so (if using an openweight model).  I could be off but I but I'm only off by a cent or 3.  Then I dove into how much gas is burnt and what is an equivalent activity... so my wife and I usually travel up to see our families like once or twice a month and I figured that if I sustained a four hour session every night, then I would burn as much in natural gas as I burn in petrol in a month.  So... all I really need to do is not go and visit my family...

I'm really struggling with my power usage...

I don't honestly know where to take this post anymore but I'm going to post it anyways... been looking at and tweaking this post for the better part of the month and been trying various things... but now things have changed and I'm struggling even more because I'm seeing first hand how MANY people seem to be using these agents and I don't like where it's gone at all...  Like, I knew people were going crazy with it but with my (apparently limited exposure) of running just one agent with no subagents in parallel made things seem tenable... not now... I'll post another blog just about oh-my-openagent...

Here's to burning all the fossil fuels....