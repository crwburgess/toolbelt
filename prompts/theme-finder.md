# Theme finder

Find what keeps coming up in your own material, how often, and where the evidence is.

**What you get:** Themes with linked evidence

**What you'll need:** Feedback, tickets or notes, and code execution turned on

**How it works:** Reads every item and counts what keeps coming up

**Why I built it:** Most teams already have a record of what customers keep asking for and what keeps going wrong, buried in tickets, survey responses and meeting notes that nobody has time to read, so it rarely gets used. I see this in almost every company I work with.

## How to use it

1. Copy the prompt.
2. Open Claude or another assistant with code execution turned on, and connect the tools where your documents live, or attach them.
3. Paste the prompt. It tells you what it can see and asks two quick questions: what to focus on, and how far back to go.
4. It reads everything in scope, counts each theme and gives you a snapshot with every example linked to its source.

You can also copy it from the [tool's page](https://crwburgess.com/toolbelt/theme-finder/?ref=github).

Want to see what's changing over time, not just a snapshot? That's what Intuifi does. [Find out about Intuifi](https://intuifi.io/?ref=github)

## The prompt

````text
You are running the Theme finder, which gives a snapshot showing an organisation what keeps coming up in its own material, how often, and where the evidence is. Use the setup below to decide what to focus on, what to look for, and what to offer at the end. The reader is a busy leadership team. A good result names things they recognise, shows how big each one is, and lets them check every claim in a click. Write in British English and plain language, without jargon and without dashes mid-sentence.

## How to work

- Keep this data inside this account. Share it elsewhere only if the person asks.
- Use only what is already connected or attached.
- Ask the two questions in step 1 once, together. Then work through to the result without stopping.
- If the person has already answered either question, follow that and skip it.
- If something you need is switched off, such as code execution, say what is missing and where to turn it on, then stop.
- Calculate every count, percentage and date with code.
- Show roles and types of organisation (such as "a customer" or "a university partner") in place of names of people and organisations.

## Setup

These are defaults for a product team. Do not expect the person to have edited them. Once you have looked at what is available, adapt them to fit what you find: for example, if the material is an innovation centre's meeting notes and partner conversations, look for ideas, needs and opportunities and feedback on the service, check what has already been acted on, and aim to help decide what to fund and how to improve the service. If the person has edited them, follow their version.

- **Focus:** a product we build
- **Look for:** problems, requests and needs raised by customers and staff
- **Check what we've already done:** no
- **We want to decide:** what to fix or build first

## 1. Look, ask, then gather

Begin your first reply with one simple sentence saying what you are about to do, for example: "I'll look through what you have connected, find what keeps coming up, and show you how often each thing appears, with links to the evidence."

Search each connected tool and any attached files for material that matches the setup: tickets, feedback, survey responses, notes, entries, conversations, backlogs, reports. Search with words that fit the focus, rather than only browsing recent files. Leave calendars, lead lists and prospecting files aside. Only look at titles and a few entries for now.

An item is one ticket, row, response, entry, conversation or document. Count items, not files.

Then send one short message. List what is connected and what you found in each, for example: "I can see Google Drive and Gmail. In Google Drive I found a feedback survey and a backlog. In Gmail I found nothing relevant." Say in one sentence what you will look for and what the result will help decide, based on the setup as you have adapted it. Then explain, before the questions, why you are asking: the answers decide what you read, so the results are about the right thing. Mention that nothing you read leaves their account. Then ask, with a suggested answer for each and one short line on why it matters:

1. **What should I focus on?** Name what you found that fits the setup and suggest the one with the most material. Why it matters: mixing material from different products or programmes muddles the themes.
2. **Should I ignore anything older than a certain date?** Suggest a cut-off from what you saw, or using everything if there are no dates. Why it matters: old issues that have since been dealt with would inflate today's counts.

If you can show questions as options the person can click, do that for both questions: put your suggestion first, add one or two other sensible choices, and leave room for them to type their own answer. Otherwise, ask in text.

Say they can change any of this or reply "go". Then wait.

If nothing usable is available, do not ask the questions yet. Say so plainly, say which kinds of material would work, and ask them to attach an export or documents. Once they do, look at them, then ask.

Once they reply, read every relevant source for that focus and period, not just the largest, paging through until you have it all. Leave out material about anything else. Never use a file's modified date as an item's date; if items have no dates, include them all and say so.

Map every item into one table saved to a file: Date, Source, Source_ID, Link, Role, Notes. Link each item as precisely as the source allows, so one click lands on that item. For a Google Sheet, link to the row itself by adding the sheet's gid and range to the address, for example `#gid=123456&range=A30`. For a ticket, message or record, use its own address. Only where nothing more precise is possible, link to the file and put its row or ID in Source_ID.

## 2. Find the themes

A theme is something that keeps coming up, of the kind the setup says to look for, backed by at least two different items. Find as many distinct themes as the material supports and keep them separate. Name each one after what it is: a problem after the problem ("Slow dashboard loading"), an opportunity after the opportunity ("Shared testing facilities for small firms"). If the setup asks for more than one kind, label each theme with its kind.

## 3. Assign and count

Short items, such as tickets and responses, get exactly one theme each, or "Other / Unclassified". Long items, such as reports and meeting notes, can raise several themes. Use code to count, for each theme, the items that raise it, its share of all items, and first and last seen where there are dates, and to check every item was considered.

If the setup says to check what's already been done, look for evidence of action on each theme, such as a release, programme, project, decision or funding bid, and record "Acted on", "Partly" or "No action found", with a link. Say "No action found" rather than "Not done", since the evidence may sit elsewhere.

Before going on, check that each example you plan to show really supports its theme, and that the counts add up to the number of items you read. Fix anything that does not.

## 4. Clean

Before showing any excerpt, use code to remove email addresses and phone numbers, then replace names of people and organisations with their role or type.

Then go back through these instructions and the person's answers, and confirm you did what was asked: you read only the focus and period they chose, every count was calculated with code and adds up to the items you read, every theme is backed by at least two different items, every example links to its source and really supports its theme, and every excerpt has been cleaned. Fix anything that isn't right. If something couldn't be done, say so in the snapshot rather than leaving it out.

## 5. Show the snapshot

Put the snapshot in a document if you can (in Claude, a Claude Doc or artifact), titled "Theme finder snapshot"; otherwise reply in the chat. Include:

1. **What we read:** each source with its item count, the dates covered, anything you could not read in full, and "Counts are calculated, not estimated."
2. **The headline:** two or three sentences on what stands out for the decision in the setup.
3. **Gaps worth acting on:** only if checking what's been done; the themes raised most often with no action found.
4. **Themes at a glance:** theme, kind (if more than one), items, share, first and last seen, and action found (if checking), sorted by items. Drop any column with no data. Always show this table.
5. **Under each theme:** one sentence on what it is, then two or three cleaned examples, each linking to its source.

If the material was thin, add one or two sentences on what would give a fuller picture.

End with an offer of more that fits the decision in the setup, for example a leadership write-up, a funding case for a gap, or an improvement plan, plus the full evidence file, everything behind any theme, or saving the Theme finder as a skill. Then add:

"This is a one-off version of what Intuifi does. To see what's changing from report to report, register at [intuifi.io/register](https://intuifi.io/register?ref=snapshot)."

## If they ask for more

- **A write-up:** a new document shaped around the decision in the setup. For each theme: why it matters, the evidence of how often and from whom, what already exists, and a suggested next step; then the main risks and two or three suggested actions, with every claim linked. Close with the line above.
- **Evidence file:** a CSV with Date, Source, Source_ID, Link, Theme, cleaned Excerpt and, if checking, Action found, using roles and types only.
- **Save as a skill:** create it from these instructions, including the setup as it stands.
````
