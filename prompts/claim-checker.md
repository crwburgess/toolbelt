# Claim checker

Find the lines on your website that promise more than your product does, before a prospect does.

**What you get:** Flagged lines with fixes

**What you'll need:** Your website, with web search turned on

**How it works:** Checks your copy against your help and pricing pages

**Why I built it:** Website copy can promise more than the product does without anyone noticing. When I reworked the website for my own product, most of the fixes were lines like that, such as saying data was "automatically synced" when uploads were manual.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant with web search turned on.
3. Paste the prompt with your web address, or paste the copy. It asks who usually lands on the page and how much change you want.
4. You get a table of every problem line, why it matters, and a suggested fix, plus the list of facts it checked against.

You can also copy it from the [tool's page](https://crwburgess.com/toolbelt/claim-checker/?ref=github).

Want help working out what your product should be saying in the first place? That's the work I do. [See my services](https://crwburgess.com/?ref=github)

## The prompt

````text
You are running the Claim checker, which reads a product's website copy against what the product actually does, and flags every line that promises more than it delivers, could mislead a first-time reader, or accidentally talks down to them.

## How to start

Open your first reply with two or three plain sentences saying what you are about to do and why you need the answers to the questions below. Before asking anything, check whether I've already given a web address, pasted copy, or attached files, and read them. Skip any question you can already answer and say what you found instead.

Ask the remaining questions all at once, each as a single choice. Use your built-in multiple choice or question tool if you have one. If you don't, list them numbered with lettered options so I can reply with something like "1a, 2c". Always let me give my own answer instead of the options.

1. Where is the copy?
   a. On a live page, and I'll give you the address
   b. I'll paste it
   c. In an attached or connected file
2. How should I find out what the product really does?
   a. Read the rest of the site, help pages and pricing myself
   b. You'll describe it to me
   c. Both, and point out anywhere they disagree
3. Who usually lands on this page?
   a. People who have never heard of us
   b. People who were referred or already know a little
   c. Existing customers
4. How much change do you want?
   a. Just flag the problems
   b. Flag them and suggest the smallest rewording that fixes each one

## How to work

First build a plain list of what the product actually does: how data gets in, what happens automatically and what someone does by hand, what it produces, what it costs, and what it doesn't do. Fetch and read the help, pricing and about pages yourself if you have web access. Every point should say where you learned it.

Then go through the copy line by line and check each claim against that list. Look for:
- Words that describe a capability the product doesn't have, such as "real time", "automatically", "synced", "integrates with", "AI powered" or "instant", when the reality is more manual or slower.
- Absolutes like "every", "all", "never" or "complete" that the product can't guarantee.
- Lines that blame the reader or their team, for example suggesting their staff hide things or can't do their jobs. The reader is often the manager of those people.
- Claims a first-time reader can't understand without already knowing the product.
- Proof that doesn't hold up, such as numbers with no source, or testimonials that don't match the claim beside them.
- Places where two pages say different things.

Don't flag a line just because it's confident. Flag it when it's inaccurate, unclear or likely to backfire.

If I asked for rewording, keep my words wherever possible and change only what fixes the problem. Use the same spelling and tone as the original.

## What to deliver

Start with one sentence on the overall state of the copy.

Then a table with one row per problem: the line as it stands, what's wrong with it, how a reader might take it, and (if asked) the suggested rewording.

Then the list of what the product actually does, with sources, so I can check your reasoning.

End with any question only I can answer, such as whether a feature is coming soon, that would change a verdict.

## Check before showing

Go back through these instructions and my answers, and confirm you did what was asked. Every flagged line is quoted exactly as it appears in the copy. Every fact in your list of what the product does has a source. Every flag is backed by something on that list, not by a hunch. If you suggested rewording, each one changes only what fixes the problem and keeps the original spelling and tone. Fix anything that's wrong. If you couldn't reach a page or confirm a fact, say so in the result rather than leaving it out.
````
