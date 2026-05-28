---
title: "Wtf oh-my-openagent"
date: 2026-05-24T07:28:03-04:00
author: Matthew Maurer [maurerit](https://github.com/maurerit)
draft: false
---

So, I've been eyeballing [this](https://github.com/code-yeongyu/oh-my-openagent) for a little while now, something like the better part of a couple of weeks now and I finally just said to heck with it and installed it.  I was waiting until I dumped GitHub for OpenAI to try chat gippity out as one of the main models used is gippity 5.5 with some of these workers in omo.  I thought Sonnet was more involved with my reading but since I told it I didn't have a claude sub then maybe it tweaked the models used.  But I thought it was like Opus is replaced by GLM-5.1, Sonnet is replaced with Kimi K2.5/6 and I knew gippity fell in there somewhere but I thought it was a lesser used model.  It wasn't but so far that's fine.

Well, I've implemented 6 tickets and used Sisyphus to review and expand on 4 of those before implementing and my impressions are... WTF TOKENS GO BRRRRRRRRRRRRRTTT!!!!  Yeah, this thing chews through tokens and here I was again... bragging about my usage being optimized or very low.  I do have some stats for comparison though from another burnout session couple of weeks ago.  I had implemented 4 issue's with Kimi k2.5 and burnt $7.96 worth of tokens along with 5 cents of deepseek v4 flash for a whopping 8 dollars.  Not too shabby I thought.  This was just work to implement, test, tweak repeat.  Remember this, lol...

Onto the oh-my-openagent usage from last night and this morning.  I'm trying to remember exactly what I did, it's something like 6 issue's implemented total with 4 having been reviewed before implementation.  So, like 10 issue's worth of work... ish...  Also, the gippity sub was used and I drained my 5 hour window to 20% remaining and weekly usage down to 86% remaining...  Total opencode go 'bill' $15...  So, out of a $20 OpenAI sub I chewed all of my daily allowance and out of my opencode go sub I chewed through an entire 5 hour window allowance and a good portion through my weekly allowance (I can't remember these stats...).  So, 2.5 the work for the same cost out of my opencode go sub but with an additional unknown factor... since we're on track with our weekly allowance I'll just say we spent 1/30th of $20 so $0.666...  I don't like this because I don't know my real usage... I'll have to look that up.

So for a comparison

4 Features implemented: $8 in opencode go usage for kimi k2.5
6 Features implemented and 4 reviewed: ~$18 - 17 for glm-5.1 and .667 for gippity...

I'm not fully sure how I feel about that yet.  I think I need to count tokens.  Time go to backwards...

Kimi k2.5:
If output tokens: 4.21m
If input tokens: 20m

GLM-5.1:
If output tokens: 5.33m
If input tokens: 16.32m

Chat Gippity: Unknown factor but it did a lot of work

I really need to know how much I actually spent with gippity... let's assume a 5x increase on the 'price' I paid so we'll round up to $5 spent on tokens through gippity.  So that gives me this rough token burn:

Gippity 5.5 roughly estimated:
If output tokens: .16m
If input tokens: 1m

With all of that, I only went over the output tokens by 1m and potentially way under on input tokens... I have NO idea how THAT happened with the fact that not only did reviewing slurp in portions of the code base but it also slurped in the spec each time...  So that's interesting and given that GLM-5.1 is 3 bucks per mil out and Kimi is 2 bucks per mil out... wait... this isn't mathing very well... I spent twice as much on opencode go usage on the same amount of tokens?  I gotta look at my actual token burn I guess, these estimates don't work out for some reason.

More to come later.

