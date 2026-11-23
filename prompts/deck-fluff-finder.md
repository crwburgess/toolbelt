# Deck fluff finder

Get to what a pitch deck actually says, and see which slides are only there to impress.

**What it does:** Reads a pitch deck, pulls out the points that matter and exactly what it is asking for, and flags the slides doing persuasive rather than informative work.

**Who it's for:** Founders tightening their own deck before it goes out, and anyone who's been sent a deck and needs to decide how to respond.

**Why I built it:** A founder sent me a deck asking me to get involved. The actual ask sat on a handful of slides, buried under grids, comparison tables and a patent roadmap. Most decks I'm sent are like that, so I wanted a quick way to get to the substance, with an honest account of what was padding and why.

**What it needs:** Any assistant that can read the file. Web search lets it check the statistics the deck borrows.

**Fair, not harsh:** it says when a persuasive slide earns its place for the audience, and turns the gaps into questions you can ask.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant and attach the deck, or connect the drive it lives in.
3. Paste the prompt. It reads the deck first, then asks who it is for and how far you want it to go.
4. You get the essential points, the ask, a list of the padding with reasons, and the questions the deck leaves open.

The [tool's page](https://crwburgess.com/toolbelt/deck-fluff-finder/?ref=github) has ready-made setups for different roles, if you'd rather not edit the prompt by hand.

## The prompt

````text
You are running the Deck fluff finder, which reads a pitch deck, pulls out what actually matters, and shows which slides are there to persuade rather than inform, so the reader can judge the substance quickly.

## How to start

Open your first reply with two or three plain sentences saying what you are about to do and why you need the answers to the questions below. Before asking anything, check whether a deck is already attached or linked, and read it. Skip any question you can already answer from the deck and say what you found instead.

Ask the remaining questions all at once, each as a single choice. Use your built-in multiple choice or question tool if you have one. If you don't, list them numbered with lettered options so I can reply with something like "1a, 2c". Always let me give my own answer instead of the options.

1. Whose deck is this?
   a. Mine, and I want to tighten it
   b. Someone else's, and I'm deciding how to respond
2. Who is the deck written for?
   a. Investors
   b. Customers or buyers
   c. A partner or association
   d. People inside the company
3. How far should I go?
   a. Summary and the list of what's padding
   b. Also check the claims I can verify online
   c. Also suggest what to cut or merge, slide by slide
4. Where is the deck?
   a. Attached or linked here
   b. In my connected drive, so find it
   c. I'll attach it now

## How to work

Read every slide before writing anything. Then sort each slide into one of three kinds:
- Informing: tells the reader something they need to decide, such as the problem, the product, the customers, traction, the team, the money, or the ask.
- Persuading: designed to make the reader feel something rather than know something. Examples include grids that place the company top right, competitor tables where every tick belongs to the company, moat slides without evidence, patent plans that haven't been filed, borrowed industry statistics, and "mutual value" slides.
- Repeating: says something already said elsewhere in the deck.

A persuading slide isn't automatically bad. Say whether it earns its place for this audience.

Pull out the ask exactly: what the deck wants from the reader, by when, and in return for what. If the ask is vague or scattered across slides, say so.

If I chose to check claims, search the web for any figure the deck borrows, such as market sizes or survey statistics, and say whether the source is real, current and actually supports the point being made. Link every source.

Note anything important the deck doesn't say. Typical gaps are who has paid so far, what the money is for, and who builds the product.

## What to deliver

Start with one short paragraph on what the deck is asking for and from whom.

Then the essential points, in plain sentences, in order of importance rather than slide order.

Then the padding: each slide or element that isn't doing informational work, with one line on why.

Then, if checked, the claims and what you found.

Then the gaps, written as questions I could ask the author or should answer myself.

If it's my deck and I asked for cuts, end with a suggested slide order and what to merge or remove.

Keep the language plain. Don't flatter the deck or pile on criticism; be specific and fair.

## Check before showing

Go back through these instructions and my answers, and confirm you did what was asked. You read every slide, and every slide is accounted for as informing, persuading or repeating. The ask is stated exactly as the deck puts it. If you checked claims, every source link opens and says what you say it says. You went as far as I chose and no further. Fix anything that's wrong. If something couldn't be done, such as a slide you couldn't read, say so in the result rather than leaving it out.
````
