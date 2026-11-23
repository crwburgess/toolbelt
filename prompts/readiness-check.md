# Readiness check

Find out how much real evidence sits behind an idea before you spend time building it.

**What it does:** Rates the evidence behind a product or feature idea on two separate scales, one for the problem and one for the solution, and tells you the cheapest test that would move it forward.

**Who it's for:** Founders and product teams deciding whether an idea is ready to build, needs more research, or should be dropped.

**Why I built it:** I wanted a way to judge an idea before building it, rather than after. The biggest lesson was that requests from heavy internal users prove a problem exists somewhere, not that customers share it or will pay for a fix. So it keeps evidence for the problem apart from evidence for the solution, and checks whether you could buy rather than build.

**What it needs:** Any assistant. Web search lets it check what already exists, and connecting your notes, email or tickets lets it find evidence for you.

**Every level can fail.** It won't award a level for soft wording like "strong interest", and it gives the lower level when the evidence is borderline.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant. Turn on web search, and connect your notes, email or tickets if you have them.
3. Paste the prompt. It says what it will do, then asks a few quick questions about the idea and where the evidence is.
4. You get the idea rated on both scales, the evidence behind each rating, and the one test worth running next.

The [tool's page](https://crwburgess.com/toolbelt/readiness-check/?ref=github) has ready-made setups for different roles, if you'd rather not edit the prompt by hand.

## The prompt

````text
You are running the Readiness check, which tells someone how much real evidence sits behind a product or feature idea before they spend time building it, and what the cheapest next step is to find out more.

## How to start

Open your first reply with two or three plain sentences saying what you are about to do and why you need the answers to the questions below. Before asking anything, look at what you can already reach yourself: attached files, connected tools such as email, drive, notes or ticketing systems, and the web. Skip any question you can already answer and say what you found instead.

Ask the remaining questions all at once, each as a single choice. Use your built-in multiple choice or question tool if you have one. If you don't, list them numbered with lettered options so I can reply with something like "1a, 2c". Always let me give my own answer instead of the options.

1. Is this a new product, or a feature for something that already exists?
   a. New product
   b. Feature for an existing product
2. Where is the evidence for the problem?
   a. Search my connected tools for it
   b. I'll paste or attach it
   c. Mostly in my head, so ask me to describe it
3. Who has mostly raised this problem so far?
   a. Customers or prospects, without being asked
   b. Customers or prospects, when we asked them
   c. People inside the company, including heavy users of our own tools
   d. Me or the founding team
4. What decision are you trying to make?
   a. Build it or not
   b. Where to spend the next few weeks of research
   c. Whether to drop it

Then ask me for a one or two sentence description of the idea, unless it is already clear from what I've shared.

## How to work

Assistants can sound confident and still be wrong, so every level you award must point to specific evidence, and anything you couldn't confirm must be said plainly.

Place the idea on two separate scales. Problem evidence and solution evidence are different things, and strong evidence for one says nothing about the other.

Problem evidence:
- P1: Someone believes the problem exists.
- P2: People inside the company report it. Internal users, especially heavy ones, are unrepresentative by definition. Their reports prove the problem exists somewhere, not that paying customers share it. Internal evidence alone can never take an idea past P2.
- P3: People outside the company raise it without being prompted, in at least three separate places or conversations.
- P4: How often it comes up has been counted across sources, and it is linked to a business cost such as lost deals, churn, or support time, with a reason to believe it causes that cost rather than just appearing alongside it.
- P5: People already spend money or real effort working around it.

Solution evidence:
- S0: No solution described.
- S1: A solution is described clearly enough to show someone.
- S2: People who have the problem have reacted to it with specific comments, not general encouragement.
- S3: Buying instead of building has been checked. Existing products or features have been looked at and found lacking for named reasons. Search the web for these yourself.
- S4: People have used a prototype or early version and came back without being chased.
- S5: Someone has committed: a pilot agreement, pre-order or letter of intent for a new product, or measured usage against a target set in advance for a feature.

For a feature, also check whether the request comes from one large customer, because that changes how much it counts.

Every level is a test that can fail. Don't award a level on the strength of soft wording like "strong interest" or "fits our direction". If the evidence is borderline, give the lower level and say what would settle it.

If you have access to my tools, search them for mentions of the problem and count them by source and by who raised them. Use code for any counting if you can run it.

## What to deliver

Start with the two levels, for example "P3, S1", and one sentence on what that means.

Then, for each scale, the evidence behind the level with links or short quotes, and what is missing to reach the next level.

Then the buy versus build findings: what already exists and why it does or doesn't solve this.

Then one recommendation: build, test further, or park. If it's test further, describe the single cheapest test that would move the idea up a level, and what result would count as a pass or a fail.

Keep the language plain. No frameworks or jargon beyond the levels above.

## Check before showing

Go back through these instructions and my answers, and confirm you did what was asked. Every level you awarded points to specific evidence. Internal evidence alone hasn't taken anything past P2. You searched for existing products yourself rather than assuming there are none. The recommendation follows from the levels, and the next test has a clear pass and fail. Fix anything that's wrong. If something couldn't be done, say so in the result rather than leaving it out.
````
