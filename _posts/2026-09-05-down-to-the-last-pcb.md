---
title: "Down to the last PCB"
date: 2026-09-05 09:00:00 -0700
categories: [MbientLab]
---

MbientLab is closing. Not dramatically, and not because anything went wrong. It
is closing the way most small companies actually end, which is quietly, after
everyone involved has slowly gotten on with their lives.

This is the part of the story that does not get written down, so I am writing it
down.

## The Work

### Everyone getting on with it (2018 – 2021)

The team did not scatter because of Covid. It had been thinning for years before
that, and every reason was a good one.

Eric went to Amazon in 2018. Stephen stopped to be a stay at home dad in 2018,
came back to work in 2020, married someone still at Intel and moved to
Sacramento. Yu moved to Las Vegas for someone he loved.

Nobody was laid off. There was no severance, because there was nothing to
soften: these are good engineers and they walked into other jobs. What was
actually happening was simpler and harder to say out loud. We had all understood
by then that MbientLab was never going to be a unicorn with a billion dollar
exit, and their lives were getting richer in other directions. That is not a
failure. It just means the company stops being the most interesting thing in
the room.

Then Covid landed on what was left.

### Running it like a startup, with nobody left (2021 – 2025)

MetaMotion RL · MetaMotion S · e-commerce · four people

I kept it running as though it were still a startup, because I wanted customers
to keep getting the treatment they had always gotten. That was the whole
intention. It was also more than one person could carry.

What was left was four of us, and the division of labour got very simple.
Sophie did HR, manufacturing, inventory and supply chain, customer support and
the money. Mark placed orders and did all the custom soldering by hand. Matt did
hardware and orders. I did customer support, software and orders.

We stopped making new hardware. From that point on we built exactly two things,
the MetaMotion RL and the MetaMotion S, over and over.

The company was profitable. It always had been. But it had changed character. In
the early years we took founder salaries that were basically pennies and pushed
every dollar back into the company. Now there was no need to reinvest like that,
just enough cash flow to keep ordering manufacturing batches and to pay
ourselves salaries that cleared poverty and not much else. We always paid
ourselves. We were never rich.

By the time I took the job at Unit21 I was down to about five hours a week on
MbientLab, on weekends and after five. It never once collided with a Unit21 or a
Gradle meeting, and I would not have let it. Those jobs paid my bills and my
insurance, and I loved the work. MbientLab took the back seat. I could afford to
let it, because it was self sustaining by then, and because anything that caught
fire, Sophie put out.

### Ryan, and one last good year (2021 – 2022)

Swift · iOS

Ryan Ferrell joined in 2021 and rebuilt the Swift APIs, and shipped a new iOS
app with them.

I was at Unit21 by then, doing well, and quietly missing writing software. Ryan
reignited something. Watching someone care about the SDKs again reminded me that
I still did.

After he left I wanted to go back through all of it, clean up the apps and the
APIs properly, finish the job. And then I started at Gradle and there was simply
no time. I was busy. It sat there for years.

### The APIs nobody asked for (2025 – 2026)

Swift 6 · Kotlin · AI-assisted

When AI tools got good, I finally had the help I needed, so I went and did it.
New Swift 6 and Kotlin APIs, written mostly by vibe coding in the evenings,
pushed to GitHub this spring and summer.

We had already decided to close by then. We were getting ready to sell out the
inventory and shut the doors. I wrote them anyway.

I do not have a business case for that. The honest reason is that it had bothered
me for four years that the SDKs were not what they should be, and for the first
time I had a way to fix it, and I did not want the last version of this thing to
be the unfinished one.

## The quiet

This is the part I would rather skip, so I will not.

If you went looking on our forum any time in the last few years, you would have
found people asking whether MbientLab was still alive, and you would have found
nobody answering. The last real post from us there is from 2022.

What happened is that the people who used to answer the forum moved on, and then
it was just me. Then Covid, and the supply chain came apart, and I was tired and
I was sick, like everyone else was. It was too much for one person. So I answered
less and less, and eventually I only answered email, because email was all I had
time for.

Customers who wrote to us got answers. Customers who posted publicly, mostly,
did not. I understand exactly how that looked from the outside, and it looked
worse than what was happening. But it was still real, and the people who asked
deserved better than silence.

## Exit

- Burnout. Mine, accumulated over about thirteen years, most of them with the
  company as a second full-time job.
- Sophie is retiring. She was the operational spine of the company for its entire
  life, and there is no version of MbientLab that works without her.
- Nobody ever tried to buy it. Not once, in thirteen years.
- So we are running the current stock down to the last PCB, and then we stop.

The exact date is somewhere between now and the first of December.

## What actually happens

There are more than two and a half million of our sensors out there, and I owe
people a plain answer about what closing means for them.

**The hardware keeps working.** Nothing switches off in the device on your desk.

**Firmware updates and reflashing stop.** Our provisioning depends on an
encrypted handshake with our servers in the US. That was a deliberate
anti-counterfeiting design and I would build it the same way again, but it has an
expiry date built into it, and this is that date. When the servers go, so does
the ability to update or reflash a board.

**MetaBase, MetaHub and MetaCloud stop.** Same reason.

**The code stays.** Everything is moving to public or private archive on GitHub,
and the last APIs get archived when we actually close. It was always open source,
and that does not change.

**The docs do not stay.** `docs.mbientlab.com` goes away.

**The store runs until the stock does.** We are not stopping cold. We are
building out the last boards and selling them.

As for the sensors themselves, honestly, I do not know. Research hardware has a
way of getting handed down between projects and outliving the lab that bought it.
I would like to think a lot of them are still collecting data somewhere, long
after anyone remembers who made them.

## Takeaways

**Quiet is a decision, even when it does not feel like one.** I never chose to
stop answering the forum. I just ran out of hours, week after week, and the
choice got made for me. From the outside there is no difference between being
overwhelmed and not caring, and the people reading only get the outside.

**A company can be profitable, well run, well loved, and still just end.** There
is a story the industry tells where companies either explode or fail. Most of
them do neither. They work fine for a decade and then the people in them are
ready to do something else.

**Building the thing properly at the end mattered to me more than it made sense
to.** I rewrote the SDKs for a company I already knew I was closing. I would do
it again.

## People

- [Ryan Ferrell](https://www.linkedin.com/in/ryanpferrell/) rebuilt the Swift
  APIs and the iOS app in 2021, and reminded me how much I missed writing
  software. That turned out to matter more than either of us knew.
- [Sophie](https://www.linkedin.com/in/sophiekassovic/) ran everything that
  actually kept the company alive, for thirteen years. She is retiring, and she
  has earned it about four times over.
- Mark, who placed the orders and hand-soldered every custom board, long after
  it would have been reasonable to.
- [Matt](https://www.linkedin.com/in/matt-baker-a85744b/), who was there for all
  of it, at the start and at the end.

Thirteen years. Two and a half million sensors. End of an era.
