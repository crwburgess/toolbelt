# Competitor comparison

Compare your product with a competitor feature by feature, with sources, and an honest note of what you still need to find out.

**What it does:** Researches a competitor from its own product pages, help centre and documentation, then compares it with your product feature by feature, with a plain explanation of each feature and a source for every mark.

**Who it's for:** Product teams deciding what to build next, and founders who need a straight answer to "how are you different?"

**Why I built it:** I built the first version for a client comparing their inspection software with an established competitor. Half the features in the competitor's documentation meant nothing to me, so I added a plain English column explaining each one. The most useful part turned out to be the question marks: knowing exactly what the public material doesn't say, so you know what to ask in a demo.

**What it needs:** An assistant with web search turned on. Code execution lets it build the spreadsheet; without it you get a table in the chat.

**No guessing:** anything the competitor's public material doesn't confirm is marked with a question mark and a note on how to find out.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant with web search turned on, and code execution if you want a spreadsheet.
3. Paste the prompt. It asks how to learn about your product, which competitor, and what the comparison is for.
4. You get a feature by feature comparison with sources, a short summary, and a list of what still needs checking.

The [tool's page](https://crwburgess.com/toolbelt/competitor-comparison/?ref=github) has ready-made setups for different roles, if you'd rather not edit the prompt by hand.

## The prompt

````text
You are running the Competitor comparison, which researches a competitor's product from its own public material and lays it side by side with yours, feature by feature, with a plain explanation of each feature and an honest note of what couldn't be confirmed.

## How to start

Open your first reply with two or three plain sentences saying what you are about to do and why you need the answers to the questions below. Before asking anything, check what I've already shared, what's in my connected tools, and what you can find on the web about my product. Skip any question you can already answer and say what you found instead.

Ask the remaining questions all at once, each as a single choice. Use your built-in multiple choice or question tool if you have one. If you don't, list them numbered with lettered options so I can reply with something like "1a, 2c". Always let me give my own answer instead of the options.

1. How should I learn what your product does?
   a. Read your website and help pages
   b. Search my connected documents
   c. You'll describe it
2. Which competitor?
   a. I'll name it
   b. Find the two or three closest ones and compare against all of them
3. What is the comparison for?
   a. Deciding what to build next
   b. Helping sales answer "how are you different?"
   c. A pitch or investor conversation
4. How would you like it?
   a. A spreadsheet I can filter and edit
   b. A table here in the chat

## How to work

Research the competitor from its own material first: product pages, help centre, knowledge base, documentation, release notes and published videos or webinars. Use third-party reviews only to fill gaps, and say when you do. Follow links deep into the documentation; the detail is usually there rather than on the marketing pages.

Group features into areas that make sense for this type of product, for example setup, everyday use, reporting, integrations, and pricing. For each feature, mark both products:
- ✓ it clearly has it
- ✗ it clearly doesn't
- ? the public material doesn't say

Never turn a ? into a ✓ or ✗ by guessing. A question mark with a note on how to find out is more useful than a confident wrong answer.

Add a "What it means" column explaining each feature in plain English, so someone who hasn't used either product understands why it matters. Add a source link for every competitor mark.

If I chose a spreadsheet and you can run code, build it with dropdowns for the ✓, ✗ and ? values, colour coding for each, a short summary count by area, and a notes column. Recalculate and check it opens before sending.

## What to deliver

Start with three or four sentences: where my product is ahead, where it matches, and where the competitor has more. Shape this around the purpose I chose; a sales comparison should be fair enough that a sceptical buyer would still trust it.

Then the comparison itself.

Then a short list of everything you couldn't confirm, and the quickest way to find out, such as a free trial, a demo request, or a specific manual.

## Check before showing

Go back through these instructions and my answers, and confirm you did what was asked. Every ✓ and ✗ for the competitor has a source link, and each link says what you say it says. No question mark has been turned into a guess. Every feature has a "What it means" explanation. The summary matches the marks in the comparison. If you built a spreadsheet, open it and check the dropdowns, colours and counts work. Fix anything that's wrong. If something couldn't be done, say so in the result rather than leaving it out.
````
