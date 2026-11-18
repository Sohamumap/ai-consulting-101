# AI Consulting 101: the 6-step method

How to help a business put AI to work, one bottleneck at a time. You don't need to code. Claude does most of the building.

From the carousel by [@sohamumap_ai](https://www.instagram.com/sohamumap_ai/). The method is adapted from Nick Saraev's AI consulting guide.

**Why now:** only 17 to 20% of US businesses used AI between December 2025 and May 2026 ([US Census Bureau](https://census.gov/library/stories/2026/05/ai-use-businesses.html)). Most of the rest have heard of it, but they don't know what it can already do for them.

---

## Step 1. Find the bottleneck

The bottleneck is the slowest step in the business. Work piles up in front of it. Speed it up and the whole business moves faster. Speed up anything else and nothing changes.

Ask the owner and each department head:

- Where does work wait the longest?
- What do you do by hand every day that feels repetitive?
- If you had one extra person for a month, where would you put them?

Then write each step of the business as a line (leads, replies, sales calls, delivery, invoicing) and next to it, how many jobs it moves in a week. The lowest number is where you start.

**Prompt for Claude:**
```
Here are my notes from talking to a business owner: [paste notes].
List every step of how this business gets and serves a customer, in order.
For each step, estimate how many jobs move through it per week and where work waits.
Tell me which step is the bottleneck and why, in plain words.
```

## Step 2. Break the goal into small tasks

Write the goal at the top (for example "more people seeing the ads"). Ask "how?" and write every answer underneath. Ask "how?" again for each answer. Stop when every line is a small, concrete action. Some of those are a perfect fit for Claude.

**Prompt for Claude:**
```
Goal: [goal]. Break it down as a tree. Under the goal, list 3 to 5 ways to reach it.
Under each, list the small concrete tasks. Mark each task: (a) Claude can do it now,
(b) Claude can do it with a connector or a tool, (c) a person has to do it.
```

## Step 3. Let Claude build it

Example: the bottleneck is ads and cost per lead.

1. Connect Claude to the client's ad account with Meta's Ads connector (`https://mcp.facebook.com/ads`, added as a custom connector in Claude). Start read-only.
2. Ask it to pull every active ad from the last 90 days and rank them by cost per lead.
3. Ask it for new hooks and headlines based on the best two.

**Prompt for Claude:**
```
Pull every active ad in this account from the last 90 days.
Rank them by cost per lead. Show the top 2 and say what they have in common.
Write 20 new hooks and 20 headlines in the same style. Don't change anything in the account.
```

## Step 4. Make it run on its own

If the client has to call you every time to run it, you are the new bottleneck.

- Save the process as a **Claude skill** (the instructions, written once).
- Run it as a **Claude routine**: routines run in Anthropic's cloud on a schedule, so nobody's laptop has to be on ([docs](https://code.claude.com/docs/en/routines)).
- No AI needed in the job? Host the script on **Modal** or **trigger.dev** on a schedule.

One client usually needs several of these.

## Step 5. Test it 10 times

The same AI setup can give a great answer once and three bad ones after it. Run it 10 times, score each run out of 10, and use the average. Change something? Run all 10 again.

| run | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | average |
|---|---|---|---|---|---|---|---|---|---|---|---|
| score | | | | | | | | | | | |

## Step 6. Teach the whole team

A system nobody uses is worth nothing. Write down how the best person on the team does the job, put it into the skill, and show everyone how to use it. Then go back to step 1 and find the next bottleneck.

---

## 3 mistakes to avoid

1. **Automating things that don't make more money.** Help with getting seen, booking calls, closing deals and selling more to existing clients.
2. **Inventing brand-new systems.** Improve a system they already use. Building new software is a developer's job.
3. **Not tracking the numbers.** Measure before you start and keep measuring, so two months in you can show what changed.

Most businesses don't need help delivering. They need more customers. Start there.

---

MIT licence.
