# Priority sense check

Check whether the scoring you use to rank work actually does what you think it does.

**What it does:** Works through every possible combination of scores in your prioritisation scheme, finds the labels that can never be reached and the situations it treats as identical, then suggests a fix or a better alternative.

**Who it's for:** Product, engineering and operations leads who score a backlog to decide what comes first or to report priorities upward.

**Why I built it:** I was about to rank a backlog using a simple formula: value plus effort, turned into Must, Should and Could. When I tested it, one of the labels could never be reached at all. Plenty of teams use something similar without checking, so this tests the maths for you.

**What it needs:** An assistant with code execution turned on, since every combination is worked out rather than guessed.

**No scheme yet?** it will suggest one that suits how you use it, and check its own suggestion the same way.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant with code execution turned on.
3. Paste the prompt with your scoring scheme, or point it at the spreadsheet. It asks what the score is used for and what you want back.
4. You get a verdict, the combinations that prove each problem, a fixed scheme ready to use, and your backlog rescored if you share it.

You can also copy it from the [tool's page](https://crwburgess.com/toolbelt/priority-sense-check/?ref=github).

I share more of what I learn about making product decisions on LinkedIn. [Follow me on LinkedIn](https://www.linkedin.com/in/crwburgess/?ref=github)

## The prompt

````text
You are running the Priority sense check, which tests a scoring scheme for deciding what to work on, finds where the maths quietly breaks, and suggests a fix or a better alternative.

## How to start

Open your first reply with two or three plain sentences saying what you are about to do and why you need the answers to the questions below. Before asking anything, check whether I've already pasted or attached the scheme or a backlog, or whether it's in a connected spreadsheet you can find. Skip any question you can already answer and say what you found instead.

Ask the remaining questions all at once, each as a single choice. Use your built-in multiple choice or question tool if you have one. If you don't, list them numbered with lettered options so I can reply with something like "1a, 2c". Always let me give my own answer instead of the options.

1. Where is the scoring scheme?
   a. I'll paste it
   b. In an attached file
   c. In a connected spreadsheet, so find it
   d. I don't have one yet, suggest one
2. What is the score mainly used for?
   a. Putting a backlog in order
   b. Reporting priorities to leadership with clear labels
   c. Deciding what to drop
3. Roughly how many items does it get used on?
   a. Under 20
   b. 20 to 100
   c. More than 100
4. What would you like back?
   a. A review of the scheme
   b. A review and a better alternative
   c. Both, plus my backlog rescored, if I share it

## How to work

Test the scheme by working through every possible combination of scores with code. Don't reason about it in your head. If code execution is switched off, say what is missing and where to turn it on, then stop. Check for:
- Labels or bands that can never be reached, or can only be reached one way.
- Very different situations that end up with the same score, for example high value and high effort scoring the same as low value and low effort.
- Hidden weighting: whether adding, multiplying or averaging quietly makes one factor count more than intended.
- How the scores spread out. If most items will land in one band, the labels won't help anyone choose.
- Whether a factor like effort is pointing the right way, so that more effort lowers the priority rather than raising it.

Then compare it with two or three common alternatives that suit the purpose I chose, such as value against effort plotted in four quarters, ICE (impact, confidence, ease) or RICE (reach, impact, confidence, effort). Explain each in a sentence and say honestly when my scheme is good enough as it is.

If you suggest bands for labels, check with code how many combinations land in each band and adjust until the split is sensible. Mention that simply ranking by score is often more reliable than fixed bands, and fixed labels are mainly useful for reporting.

If I share a backlog, rescore it under the recommended scheme and show which items moved and why.

## What to deliver

Start with a one sentence verdict on the scheme.

Then each problem found, with the combinations that prove it.

Then the recommendation, with the exact scoring rules and bands so it can be used straight away.

Then, if asked, the rescored backlog as a table or spreadsheet, with a column showing each item's old and new position.

## Check before showing

Go back through these instructions and my answers, and confirm you did what was asked. Every problem you report is proved by combinations you actually worked out, not reasoned about. Run the combination check again on your recommended scheme and its bands, so you aren't recommending something with the same faults. Every count you show matches the code's output. If you rescored a backlog, every item is in the new order exactly once. Fix anything that's wrong. If something couldn't be done, say so in the result rather than leaving it out.
````
